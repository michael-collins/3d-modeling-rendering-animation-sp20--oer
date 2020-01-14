<table class="feedback">
  <tr class="table-labels">
    <td class="table-label">% Earned</td>
    <td class="table-label">Criterion 1 Feedback</td> 
    <td class="table-label">Criterion 2 Feedback</td>
  </tr>
{% for feedback in site.data.simple-assignment-default-feedback %}
  <tr class="feedback-data">
    <td>{{ feedback.percent-earned }}</td>
    <td>{{ feedback.criterion-1-feedback }}</td> 
    <td>{{ feedback.criterion-2-feedback }}</td>
  </tr>
{% endfor %}
</table>
