<table class="feedback">
  <tr class="table-labels">
    <td class="table-label">Criterion</td>
    <td class="table-label">Description</td>
    <td class="table-label">Value</td>
  </tr>
 
{% for item in site.data.project-rubric %}
  <tr class="feedback-data">
    <td>{{ item.Criterion }}</td>
    <td>{{ item.CriterionDescription }}</td>
    <td>{{ item.CriterionTotalValue }}</td>
  </tr>
{% endfor %}
</table>