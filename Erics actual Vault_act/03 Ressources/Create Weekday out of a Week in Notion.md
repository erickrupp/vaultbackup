---
status: finalised
training:
tags:
  - notion_tipps
type:
  - "[[tipp]]"
---

# **Create Weekday out of a Week in Notion**
## **2022-02-26 10:14**

The Weekday can be automatically created out of a date-property by inserting a new formula property for this weekday and in this property add the following formula:

formatDate(prop("Date"), "dddd") 

whereas: 'prop("Date")' is referenced to the date field for which the weekday is requested. So keep this in mind and change the word 'Date' into the name of your property


### Reference
[[Notion]]
[[Computertipps]] 