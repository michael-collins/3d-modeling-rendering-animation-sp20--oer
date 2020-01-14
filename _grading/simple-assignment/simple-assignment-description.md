---
title: Grading Criteria
subtitle: Exercise Feedback
layout: default
---
### Example Grade Report
<table class="rubric">
  <tr class="table-labels">
    <td class="table-label">Criterion</td>
    <td class="table-label">Earned Value</td> 
    <td class="table-label">Total Possible Value</td>
  </tr>
{% for rubric in site.data.simple-assignment-rubric %}
  <tr class="rubric-data">
    <td>{{ rubric.criterion-id }}</td>
    <td>{{ rubric.earned-value }}</td> 
    <td>{{ rubric.total-possible-value }}</td>
  </tr>
{% endfor %}
</table>

### Feedback Details
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
