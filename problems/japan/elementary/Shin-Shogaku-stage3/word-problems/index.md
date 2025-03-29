---
layout: default
title: Word Problems Index
---

# 🧠 Word Problems for Stage 3

Welcome to the collection of mathematical word problems for advanced learners!  
Choose your favorite category and challenge yourself at **Standard** or **Advanced** level!

---

{% assign categories = 
  "Elimination,Age,Difference&Spacing,Crane&Turtle,Salt-Solution&Profit,Equivalent,WorkRate,DistributionRatio,MultipleRatio,Newton-Type" | split: "," %}

{% for category in categories %}
## 🔹 {{ category }}

<div style="margin-left: 1rem;">

### 🧩 Standard Level

<table>
  <tr>
    {% for i in (1..6) %}
      {% assign filename = "./" | append: category | append: "/standard-level-problem-" | append: i | append: ".html" %}
      <td>
        {% if site.static_files | where: "path", filename | size > 0 %}
          <a href="{{ filename }}">Problem {{ i }}</a>
        {% else %}
          <span style="color:gray;">Coming Soon</span>
        {% endif %}
      </td>
    {% endfor %}
  </tr>
</table>


### 🚀 Advanced Level

<table>
  <tr>
    {% for i in (1..6) %}
      {% assign filename = "./" | append: category | append: "/advanced-level-problem-" | append: i | append: ".html" %}
      <td>
        {% if site.static_files | where: "path", filename | size > 0 %}
          <a href="{{ filename }}">Problem {{ i }}</a>
        {% else %}
          <span style="color:gray;">Coming Soon</span>
        {% endif %}
      </td>
    {% endfor %}
  </tr>
</table>



</div>

---

{% endfor %}
