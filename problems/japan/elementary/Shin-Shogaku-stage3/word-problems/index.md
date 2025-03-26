---
layout: default
title: Word Problems Index
---

# 🧠 Word Problems for Stage 3

Welcome to the collection of mathematical word problems for advanced learners!  
Choose your favorite category and challenge yourself at **Standard** or **Advanced** level!

---

{% assign categories = 
  "Elimination problem,Age Problem,Difference & Spacing Calculations,Crane and Turtle Calculations,Salt Solution & Profit Calculations,Equivalent Proportion,Work Rate Problem,Distribution Ratio Problem,Multiple-Based Ratio,Newton-Type" | split: "," %}

{% for category in categories %}
## 🔹 {{ category }}

<div style="margin-left: 1rem;">

### 🧩 Standard Level

<table>
  <tr>
    <td><a href="./{{ category }}/Standard Level – Problem 1.md">Problem 1</a></td>
    <td><a href="./{{ category }}/Standard Level – Problem 2.md">Problem 2</a></td>
    <td><a href="./{{ category }}/Standard Level – Problem 3.md">Problem 3</a></td>
  </tr>
</table>

### 🚀 Advanced Level

- [Problem 1](./{{ category }}/Advanced Level – Problem 1.md)
- [Problem 2](./{{ category }}/Advanced Level – Problem 2.md)
- [Problem 3](./{{ category }}/Advanced Level – Problem 3.md)

</div>

---

{% endfor %}
