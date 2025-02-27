---
<%*
let title = await tp.system.prompt("Snippet Name")
let given_tags = await tp.system.prompt("Tags (js, web)")
let lang = await tp.system.prompt("Programming Language:")
let now = tp.date.now()

let tags = given_tags.split(",")
tp.file.title = await tp.file.rename(`Snippet-${title}`)
tp.file.tags = tags.includes('snippet') ? tags : [...tags, 'snippet']
%>
date: <%* now %>
language: <%* tR += lang %>
tags: [<% tp.file.tags %>]
---

## Description
Provide a brief explanation of the snippet.  
- What problem does it solve?  
- When and how should it be used?

## Code
```<%* tR += lang %>
<!-- Paste your code snippet here -->
