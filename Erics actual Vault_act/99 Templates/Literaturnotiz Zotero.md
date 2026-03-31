---
note: tvz 
training:
tags: literatur
title: "{{title}}"
author: {{authors}} {{directors}}
itemType: {{itemType}}
media: 
 - buch
type: "[[litnote]]"
verlag: "{{publisher}}"
veröffentlicht: {{date | format("YYYY")}}
heruntergeladen am: {{dateAdded | format("YYYY-MM-DD")}}
isbn: {{ISBN}}
status: new 
project:
area:
context:
---

# {{title}}

Zotero-Link: {{pdfZoteroLink}}
Buchtitel: {{bibliography}}

---
## Abstract
>[!ABSTRACT]-
> {{abstractNote}}

---
## Notes from Zotero
{%- if markdownNotes %} 
{{markdownNotes}} 
{%- endif -%}
_
 
___

## Annotations 

{% for annotation in annotations -%} 
    {%- if annotation.annotatedText -%} 
    {{annotation.annotatedText}} {% if annotation.color %} {{annotation.colorCategory}} {{annotation.type | capitalize}} {% else %} {{annotation.type | capitalize}} {% endif %}[Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}}) 
    {%- endif %} 
    {%- if annotation.imageRelativePath -%}
    ![[{{annotation.imageRelativePath}}]] {%- endif %} 
{% if annotation.comment %} 
{{annotation.comment}} 
{% endif %} 
{% endfor -%}


## Reference
**OUTLINKS**
![[Outlinks.base]]


**BACKLINKS**
![[Backlinks.base]]