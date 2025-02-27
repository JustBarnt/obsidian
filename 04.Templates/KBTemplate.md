---
<%*
let title = await tp.system.prompt("Article Name")
let given_tags = await tp.system.prompt("Tags: (low-level,c++)")

let tags = given_tags.split(",")
tp.file.title = await tp.file.rename(title)
tp.file.tags = tags.includes('kb') ? tags : [...tags, 'kb']
_%>

date: {{date:YYYY-MM-DD}}
tags: <% tp.file.tags %>
---

## Summary
Provide a concise overview of the article. Explain what the reader will learn and why it's important.

## Introduction
Introduce the topic and its relevance. Provide context and state the purpose of the article.

## Background / Context
Detail any necessary background information. Include definitions, historical context, or related concepts that set the stage for the main content.

## Main Content
Break down the topic into digestible sections. Consider using subheadings for clarity:
- **Overview:**  
  Explain the general idea or concept.
- **In-Depth Analysis:**  
  Dive into the details, present data, code samples, or technical information as needed.
- **Practical Applications:**  
  Describe real-world use cases, best practices, or how to implement the concepts discussed.

## Visuals / Diagrams
If applicable, include images, diagrams, or charts to illustrate key points:
- Example:  
  ![Diagram Description](path/to/diagram.png)

## Conclusion
Summarize the key takeaways of the article. Reinforce the main points and suggest next steps or further exploration if necessary.

## References & Further Reading
List any sources, external references, or additional resources that can provide further insight:
- [Reference Title](https://example.com)
- [Another Resource](https://example.com)

---

*Created on {{date:YYYY-MM-DD}}*
