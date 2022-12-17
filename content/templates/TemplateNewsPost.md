---
title: "{{title}}"
date-created: {{date:YYYY-MM-DD}}
day-of-week-created: {{date:ddd}}
date-updated: 
aliases: []
tags: [NewsPost]
status: stable
---

# {{title}}

| Date     | Site | External Link                          | 
| -------- | ---- | -------------------------------------- |
| {{date}} |      | [*{{title}}*]<% tp.file.cursor(1) %> |

## Contributors
- <% tp.file.cursor(2) %>

## Summary
> <% tp.file.cursor(3) %>

| Date | Site | Title / Internal Link | 
| ---- | ---- | --------------------- |
<% tp.file.cursor(4) %>
## Players
- <% tp.file.cursor(5) %>

## Staff
- <% tp.file.cursor(6) %>

## Notes and Quotes
<% tp.file.cursor(7) %>
