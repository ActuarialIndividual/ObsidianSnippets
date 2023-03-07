<%*
/*
```javascript
*/
const type = await tp.system.suggester(["Note","Help","Tip","Summary","Tldr","Warning","Bug"],["note","help","tip","summary","tldr","warning","bug"])
const title = await tp.system.prompt("Title")

if(title === undefined) {
title2 = type
} else {
title2 = title
}

const template = await tp.file.include("[[callout]]")
const x1 = template.replaceAll("$TYPE",type).replaceAll("$TITLE",title2)

tp.file.cursor_append(x1)


/*
```
*/
%>

