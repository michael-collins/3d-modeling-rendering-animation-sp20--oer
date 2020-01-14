<table class="feedback">
  <tr class="table-labels">
    <td class="table-label">Date</td>
    <td class="table-label">Topic</td>
    <td class="table-label">Due</td>
  </tr>
 
{% for item in site.data.calendarSP19 %}
  <tr class="feedback-data">
    <td>{{ item.Date }}</td>
    <td>{{ item.Topic }}</td>
    <td>{{ item.Due }}</td>
  </tr>
{% endfor %}
</table>
