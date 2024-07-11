---
title: Home 
---

# The Koslicki Lab at Pennsylvania State University
The Koslicki lab focuses on computational biology. We are interested in developing efficient, mathematically sound approaches to extract insight from omics data. This puts our research squarely at the intersection of biology, mathematics, and computer science. We are particularly interested in the entire arc of developing computational biology methods: rigorous mathematical justification of a method, implementing the method into a tool usable by the community, applying the tool to pressing scientific problems, and finally using the results to inform further development of computational techniques.

<div class="item2">
  <p style='text-align: center; font-size: 18px'> Recent News About Our Lab</p>
  {% for article in site.data.news limit:2 %}
  <p><em> {{ article.date }} </em></p>
  <p>{{ article.headline }}</p>
  {% endfor %}
  <p><a href="{{ 'allnews/allnews.html' | relative_url }}">... see all News</a></p>
</div>


<!-- section break -->

{%
  include figure.html
  image="images/team/lab_photo_smaller.png"
  caption="Part of our team"
  width="100%" 
%}

<!-- section break -->
# Research Direction

{% capture text %}
Computational data-driven research focuses on developing and applying computational methods across various types of omics datasets. Such research is performed in a new type of laboratory, often called a dry lab. Our team designs, develops and applies novel and robust data-driven, computational approaches that will accelerate the diffusion of genomics and biomedical data into translational research and education.
{% endcapture %}

{%
  include feature.html
  image="images/direction1_image.jpg"
  link="research"
  heading="Algorithm Development or Mathematical Theory"
  text=text
%}

{% capture text %}
We believe in data analysis transparency, effective sharing, reproducibility, software usability, and archival stability to foster a sustainable data science ecosystem in biomedical research.
{% endcapture %}

{%
  include feature.html
  image="images/direction2_image.jpg"
  link="research"
  heading="Reasoning Over Large Knowledge Graphs"
  text=text
%}

{% capture text %}
We are a team of enthusiastic researchers aimed to combine open omics data with robust bioinformatics methods to enable novel biological discoveries. We are committed to ensuring an inclusive and supportive environment. We also believe in empowering the members of our team with necessary bioinformatics training and support, allowing them to make important contributions to the fields of biomedical research.
{% endcapture %}

{%
  include feature.html
  image="images/direction3_image.jpg"
  link="research"
  heading="Metagenomics Research"
  text=text
%}
