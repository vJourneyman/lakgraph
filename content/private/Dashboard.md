---
title: "Dashboard"
date-created: 2022-10-11
day-of-week-created: Tue
date-updated: 
aliases: []
tags: []
status: stable
---

# Dashboard


```dataview
TABLE status, tags
  FROM #NewsPost OR #NewsSite OR #Player OR #Staff OR #PodcastEpisode AND -"templates"
sort tag, status
```
