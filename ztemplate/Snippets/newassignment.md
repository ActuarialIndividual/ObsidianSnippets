<%* 
/*
```javascript
*/

if (tp.frontmatter.subject === undefined) {
	sub = await tp.system.prompt("Subject Code")
} else {
	sub = tp.frontmatter.subject
}

const num = await tp.system.prompt("Assignment No.")
const path = "Assignments/"+sub+" A"+num

if (tp.file.exists(path)) {
	Notice("Warning: Assignment file already exists")
	return;
}

const dd = await tp.system.prompt("Due Date")

const template = await tp.file.include("[[assignment]]")
const x1 = template.replaceAll("$SUBJECT",sub).replaceAll("$DUEDATE",dd)

tp.file.create_new(x1, path, true)

/*
```
*/
%>