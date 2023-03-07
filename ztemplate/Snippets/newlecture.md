<%* 
/*
```javascript
*/
const fie = tp.frontmatter.field
const name = await tp.system.prompt("New Lecture")

if (tp.frontmatter.subject === undefined) {
	sub = await tp.system.prompt("Subject Code")
} else {
	sub = tp.frontmatter.subject
	tp.file.cursor_append("---"+"\n#### [["+name+"]]"+"\n\n![["+name+"#Summary]]")
};

const template = await tp.file.include("[[lecture]]")
const x1 = template.replaceAll("$SUBJECT",sub).replaceAll("$FIELD",fie).replaceAll("$NAME",name)

tp.file.create_new(x1, "Lecture Notes/"+sub+"/"+name, true)
/*
```
*/
%>