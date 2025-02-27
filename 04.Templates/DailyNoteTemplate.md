---
<%*
const today = tp.date.now()
const yesterday = tp.date.yesterday()
console.log(await tp.file.find_tfile(yesterday))
const tags = ["DailyNotes"]
tp.file.tags = tags
_%>
tags: [<% tp.file.tags %>]
CurrentDate: <% today %>
PreviousDate: <% yesterday %>
---
<%* if (tp.file.find_tfile(yesterday) != null){ %>
Previous Daily Note
[[<%* tR += yesterday %>]]
<%*} %>

