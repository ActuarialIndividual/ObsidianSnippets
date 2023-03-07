<%*
/*
```javascript
*/
const lecture = tp.file.title
const subject = tp.frontmatter.subject
const field = tp.frontmatter.field

const name = await tp.system.prompt("Definition")

tp.file.cursor_append("\n\n![["+name+"#Definition]]") 

const template = await tp.file.include("[[definition]]")
const x1 = template.replaceAll("$SUBJECT",subject).replaceAll("$FIELD",field).replaceAll("$LECTURE",lecture)

tp.file.create_new(x1, "Definitions/"+name, true)
/*
```
*/
%>
