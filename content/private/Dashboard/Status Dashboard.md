---

database-plugin: basic

---

```yaml:dbfolder
name: dashboard
description: status dashboard
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 2
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
  status:
    input: select
    accessorKey: status
    key: status
    id: status
    label: status
    position: 100
    isSorted: true
    isSortedDesc: false
    sortIndex: 0
    skipPersist: false
    isHidden: false
    options:
      - { label: "unstarted", backgroundColor: "hsl(246, 95%, 90%)"}
      - { label: "stable", backgroundColor: "hsl(80, 95%, 90%)"}
      - { label: "needs-draft-content", backgroundColor: "hsl(240, 95%, 90%)"}
      - { label: "raw-transcript", backgroundColor: "hsl(108, 95%, 90%)"}
      - { label: "NoNotes", backgroundColor: "hsl(43, 95%, 90%)"}
      - { label: "NeedsImprovement", backgroundColor: "hsl(246, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
  date-created:
    input: text
    accessorKey: date-created
    key: date-created
    id: date-created
    label: date-created
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: 1
    isSorted: true
    isSortedDesc: false
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
  tags:
    input: tags
    accessorKey: tags
    key: tags
    id: tags
    label: tags
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    isSorted: false
    isSortedDesc: false
    options:
      - { label: "NewsPost", backgroundColor: "hsl(40, 95%, 90%)"}
      - { label: "Status/New,Staff", backgroundColor: "hsl(55, 95%, 90%)"}
      - { label: "NewsSite", backgroundColor: "hsl(9, 95%, 90%)"}
      - { label: "Status/New,Player", backgroundColor: "hsl(161, 95%, 90%)"}
      - { label: "PodcastEpisode", backgroundColor: "hsl(7, 95%, 90%)"}
      - { label: "NewsPost,SalaryCap", backgroundColor: "hsl(272, 95%, 90%)"}
      - { label: "Player", backgroundColor: "hsl(190, 95%, 90%)"}
      - { label: "NewsPost,Podcast", backgroundColor: "hsl(67, 95%, 90%)"}
      - { label: "Status/stable,Staff", backgroundColor: "hsl(299, 95%, 90%)"}
      - { label: "Status/Stable,Player", backgroundColor: "hsl(319, 95%, 90%)"}
      - { label: "Status/NeedsImprovement,Player", backgroundColor: "hsl(77, 95%, 90%)"}
      - { label: "NewsPost,PowerPlay", backgroundColor: "hsl(250, 95%, 90%)"}
      - { label: "PodcastEpisode,LiteratureNote", backgroundColor: "hsl(295, 95%, 90%)"}
      - { label: "Status/New", backgroundColor: "hsl(133, 95%, 90%)"}
      - { label: "Staff", backgroundColor: "hsl(274, 95%, 90%)"}
      - { label: "LiteratureNote", backgroundColor: "hsl(196, 95%, 90%)"}
      - { label: "Podcast", backgroundColor: "hsl(8, 95%, 90%)"}
      - { label: "Status/Stable", backgroundColor: "hsl(114, 95%, 90%)"}
      - { label: "Status/stable", backgroundColor: "hsl(151, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: false
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  source_data: query
  source_form_result: "FROM #NewsPost OR #NewsSite OR #Player OR #Staff OR #PodcastEpisode AND -\"templates\" AND -\"private\" AND -\"reference\""
  source_destination_path: /
  frontmatter_quote_wrap: false
  row_templates_folder: /
  current_row_template: 
  pagination_size: 10
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: top
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
filters:
  enabled: false
  conditions:
```