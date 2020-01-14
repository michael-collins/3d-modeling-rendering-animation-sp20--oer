<table class="feedback">
  <tr class="table-labels">
    <td class="table-label">% Earned</td>
    <td class="table-label">Criterion 1 Feedback</td>
    <td class="table-label">Criterion 2 Feedback</td>
  </tr>
 
{% for item in site.data.exercise-rubric %}
  <tr class="feedback-data">
    <td>{{ item.Earned }}</td>
    <td>{{ item.Criterion1 }}</td>
    <td>{{ item.Criterion2 }}</td>
  </tr>
{% endfor %}
</table>