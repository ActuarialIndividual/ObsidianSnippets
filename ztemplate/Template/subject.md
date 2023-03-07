---
aliases:
type: subject
subject: <% tp.file.title %>
field:
period:
---

# Lecture Notes



# To-Do's

```dataview
TASK
WHERE contains(subject,"<% tp.file.title %>")
```


# Definitions

```dataview
TABLE difficulty as "Difficulty"
WHERE contains(subject,"<% tp.file.title %>") and type = "definition"
SORT difficulty DESC
```
