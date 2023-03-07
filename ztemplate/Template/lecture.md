---
date: <% tp.date.now() %>
type: lecture
subject: $SUBJECT
field: $FIELD
---

> [[$SUBJECT]]

# Summary

> [!summary]- Key Concepts
> ```dataview
> LIST difficulty
> FROM "Definitions"
> WHERE contains(lecture,"$NAME")
> SORT difficulty DESC
> ```


# Overview

