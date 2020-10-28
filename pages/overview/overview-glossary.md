---
title: Glossary
keywords: abbreviations, definitions, glossaries, terms
tags: [overview]
sidebar: overview_sidebar
permalink: overview-glossary.html
summary: "Glossary of terms used in this Usage Guide"
toc: false
---

A further glossary of common terms and abbreviations used throughout the documentation can be found on the [NHS Digital developer hub](https://digital.nhs.uk/developer/guides-and-documentation/glossary-of-developer-terms).


{% for item in site.data.glossary %}  

#### {{ item.keyword }}
{% if item.expansion %}
**{{item.expansion}}**
{% endif %}
  
{% if item.definition %}
{{item.definition}}
{% endif %}

{% endfor %}
