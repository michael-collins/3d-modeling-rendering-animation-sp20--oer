{% if include.mode == "accordion" or include.mode == null %}
    <ul class="collapsible popout" data-collapsible="accordion">
    
    {% assign all_items = "" | split: "" %}
    {% for item in site.data.schedule.assignments %}
        {% assign all_items = all_items | push: item %}
    {% endfor %}
    {% comment %}
    {% for item in site.data.schedule.assignments %}
        {% for  milestones in item.milestones %}
            {% assign all_items = all_items | push: item %}
        {% endfor %}
    {% endfor %}
    {% endcomment %}
    {% for item in site.data.schedule.agendas %}
        {% assign all_items = all_items | push: item %}
    {% endfor %}
    
     {% comment %}
     ### Sort an array of all agenda, assignments, and presentations
     {% endcomment %}
    {% assign sorted-items = all_items | sort: 'posted-date-iso' | reverse | where: "published", true %}
    {% for item in sorted-items %}
        {% capture date %}{{ item.posted-date-iso | date: '%m%d%Y' }}{% endcapture %}
        {% assign itemDate = item.posted-date-iso | date: "%m%d%Y" %}
        {% if itemDate != myDate %}
            {% unless forloop.first %}
                </div>
            </li>
            {% endunless %}
            <li>
                <div class="collapsible-header">
                    <h5 class="post-date">{{ item.posted-date-iso | date: "%A, %B %e, %Y" }}</h5>  
                </div>
                <div class="collapsible-body">
            {% assign myDate = itemDate %}
        {% endif %}

            <h5 class="post-title"><a href="{{ item.doc | prepend: site.baseurl }}"><span class="post-title">{{ item.title }}</span></a><span class="post-type {{item.categories}}"> ( {{item.categories}} )</span></h5>
            

        {% if forloop.last %}
        </li>
        {% endif %}
    {% endfor %}
    </ul>


{% elsif include.mode == "table" %}
    <table class="striped schedule">
        {% comment %} <thead>
          <tr>
              <th>Date</th>
              <th>Assignment</th>
          </tr>
        </thead> {% endcomment %}
            <tbody>
            {% comment %} #### BUILD ARRAY ####
            ## Combine all agenda, assignments, and presentations into a single array
            {% endcomment %}
            {% assign all_items = "" | split: "" %}
            {% for item in site.data.schedule.assignments %}
                {% assign all_items = all_items | push: item %}
            {% endfor %}
            {% for item in site.data.schedule.agendas %}
                {% assign all_items = all_items | push: item %}
            {% endfor %}
            {% for item in site.data.schedule.presentations %}
                {% assign all_items = all_items | push: item %}
            {% endfor %}
            {% comment %} #### END BUILD ARRAY #### {% endcomment %}
            
            {% comment %} #### SORT ARRAY ####            
            ## Sort an array of all agenda, assignments, and presentations
            {% endcomment %}
            {% assign sorted-items = all_items | sort: 'posted-date-iso' | reverse | where: "published", true %}
            {% for item in sorted-items %}
            {% capture date %}{{ item.posted-date-iso | date: '%m%d%Y' }}{% endcapture %}
            {% assign itemDate = item.posted-date-iso | date: "%m%d%Y" %}
            {% comment %} #### END SORT ARRAY #### {% endcomment %}
            
            {% comment %} #### BUILD TABLE BASED ON UNIQUE POST DATES #### 
            ### Does the date in the array item match the current item's date? If not, print it as a new table item 
            {% endcomment %}
            {% if itemDate != myDate %}
                {% unless forloop.first %}        
                {% endunless %}
                <tr>
                    <td>
                        <h5 class="post-date"><strong>{{ item.posted-date-iso | date: "%A" }}</strong><br><span class="no-break">{{ item.posted-date-iso | date: "%b %e" }}</span><br>{{ item.posted-date-iso | date: "%Y" }}</h5>
                        {% assign myDate = itemDate %}
                    </td>
                    <td>
            {% endif %}
            {% if item.type contains "exercise" %}
                {% for assignment in site.assignments %}
                    {% if item.id == assignment.slug %}
                        <div class="post-wrapper">
                            <i class="fas fa-file-alt"></i>
                            <h5 class="post-title"><a href="{{ item.doc | prepend: site.baseurl }}" class="has-icon"><span class="post-title">{{ item.title }}: {{ assignment.title }}</span></a></h5>
                            <div class="schedule-post-links">
                                <p class="schedule-due-date"><strong>Due date:</strong> {{ item.due-date-iso | date: "%B %e at %I:%M%P %Z" }}</p>
                                {% comment %} <i class="fas fa-file-alt"></i><a href="{{ item.doc | prepend: site.baseurl }}" target="_blank"><span class="schedule-documentation">Instructions</span></a> {% endcomment %}
                                <i class="fas fa-cloud-upload-alt"></i><a href="{{ item.dropbox-url }}" target="_blank"><span class="schedule-dropbox">Dropbox</span></a>
                            </div>
                        </div>
                    {% endif %}
                {% endfor %}
            {% elsif item.type contains "project" %}
                {% for assignment in site.assignments %}{% comment %} ## Match assignment.yml item with assignment collection item {% endcomment %}
                    {% if item.id == assignment.slug %} {% comment %} ## If item's ID equals assignment FILENAME {% endcomment %}
                        <div class="post-wrapper">
                        <i class="fas fa-file-alt"></i>
                            <h5 class="post-title"><a href="{{ item.doc | prepend: site.baseurl }}"" class="has-icon"><span class="post-title">{{ item.title }}</span></a></h5>
                            <div class="schedule-post-links">
                                {% comment %} <i class="fas fa-file-alt"></i><a href="{{ item.doc | prepend: site.baseurl }}" target="_blank"><span class="schedule-documentation">Instructions</span></a> {% endcomment %}
                                {% for milestone in item.milestones %}
                                    <h6>{{milestone.title}}</h6>
                                    <p class="schedule-due-date"><strong>Due date:</strong> {{ milestone.due-date-iso | date: "%B %e at %I:%M%P %Z" }}</p>
                                    <i class="fas fa-cloud-upload-alt"></i><a href="{{ milestone.dropbox-url }}" target="_blank"><span class="schedule-dropbox">Dropbox</span></a>
                                    {% if forloop.last  == true %}
                                    {% else %}
                                    <hr>
                                    {% endif %}
                                {% endfor %}
                            </div>
                        </div>
                    {% endif %}
                {% endfor %}
            {% elsif item.type contains "agenda" %}
                {% for agenda in site.agendas %}
                    {% if item.id == agenda.slug %}
                    <div class="post-wrapper">
                    <i class="fas fa-clipboard"></i>
                        <h5 class="post-title"><a href="{{ item.doc | prepend: site.baseurl }}" class="has-icon"><span class="post-title">{{ agenda.title }}</span></a></h5>
                    </div>
                    {% endif %}
                {% endfor %}
            {% elsif item.type contains "presentation" %}
                {% for presentation in site.presentations %}
                    {% if item.id == presentation.slug %}
                        <div class="post-wrapper">
                        <i class="fas fa-desktop"></i>
                            <h5 class="post-title"><a href="{{ item.doc | prepend: site.baseurl }}" class="has-icon"><span class="post-title">{{ presentation.title }}</span></a></h5>
                        </div>
                    {% endif %}
                {% endfor %}
            {% endif %}
            
                    
        {% if forloop.last %}
        </td>
                </tr>
        {% endif %}
        {% comment %} #### ENDBUILD TABLE BASED ON UNIQUE POST DATES #### {% endcomment %}

        {% endfor %}
        </tbody>
    </table>
{% endif %}