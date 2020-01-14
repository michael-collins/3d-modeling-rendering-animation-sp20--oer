{% if include.mode == "accordion" or include.mode == null %}
    <ul class="collapsible popout" data-collapsible="accordion">
    {% for post in site.posts %}
    {% capture date %}{{ post.date | date: '%m%d%Y' }}{% endcapture %}
    {% assign currentDate = post.date | date: "%m%d%Y" %}
    {% if currentDate != myDate %}
        {% unless forloop.first %}
            </div>
        </li>
        {% endunless %}
        <li>
            <div class="collapsible-header">
                <h5 class="post-date">{{ post.date | date: "%A, %B %e, %Y" }}</h5>  
            </div>
            <div class="collapsible-body">
        {% assign myDate = currentDate %}
    {% endif %}

        <h5 class="post-title"><a href="{{ post.url | prepend: site.baseurl }}"><span class="post-title">{{ post.title }}</span></a><span class="post-type {{post.categories}}"> ( {{post.categories}} )</span></h5>
        

    {% if forloop.last %}
    </li>
    {% endif %}
    {% endfor %}
    </ul>


{% elsif include.mode == "table" %}
    <table class="striped">
        <thead>
          <tr>
              <th>Date</th>
              <th>Assignment</th>
          </tr>
        </thead>
            <tbody>
            {% for post in site.posts %}
            {% capture date %}{{ post.date | date: '%m%d%Y' }}{% endcapture %}
            {% assign currentDate = post.date | date: "%m%d%Y" %}
            {% if currentDate != myDate %}
                {% unless forloop.first %}
                    
                {% endunless %}
                <tr>
                    <td>
                        <h5 class="post-date">{{ post.date | date: "%A, %B %e, %Y" }}</h5>
                        {% assign myDate = currentDate %}
                    </td>
                    <td>
                        

            {% endif %}
            <h5 class="post-title"><a href="{{ post.url | prepend: site.baseurl }}"><span class="post-title">{{ post.title }}</span></a><span class="post-type {{post.categories}}"> ( {{post.categories}} )</span></h5>
            {% if post.categories contains "exercise" %}
                <div class="schedule-post-links">
                <p class="schedule-due-date"><strong>Due date:</strong> {{site.assignments.[post.assignment].due-date}}</p>
                <i class="far fa-file-alt"></i><a href="{{ site.assignments.[post.assignment].doc | prepend: site.baseurl }}" target="_blank"><span class="schedule-documentation">Instructions</span></a>
                <i class="fas fa-cloud-upload-alt"></i><a href="{{ site.assignments.[post.assignment].dropbox-url }}" target="_blank"><span class="schedule-dropbox">Dropbox</span></a>
                </div>
            {% endif %}
            
                    
        {% if forloop.last %}
        </td>
                </tr>
        {% endif %}
        {% endfor %}
        </tbody>
    </table>
{% endif %}