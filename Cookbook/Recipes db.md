---

database-plugin: basic

---

```yaml:dbfolder
name: Recipe Cookbook
description: Recipe database
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
    position: 1
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      content_vertical_alignment: align-top
  made_it:
    input: checkbox
    accessorKey: made_it
    key: made_it
    id: made_it
    label: made it
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  rating:
    input: number
    accessorKey: rating
    key: rating
    id: rating
    label: rating
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      content_vertical_alignment: align-top
  course:
    input: select
    accessorKey: course
    key: course
    id: course
    label: course
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Dessert", value: "Dessert", color: "hsl(219, 95%, 90%)"}
      - { label: "Main Course", value: "Main Course", color: "hsl(27, 95%, 90%)"}
      - { label: "Bread", value: "Bread", color: "hsl(91, 95%, 90%)"}
      - { label: "Side Dish", value: "Side Dish", color: "hsl(342, 95%, 90%)"}
      - { label: "Preparation", value: "Preparation", color: "hsl(324, 95%, 90%)"}
      - { label: "Drink", value: "Drink", color: "hsl(47, 95%, 90%)"}
      - { label: "Breakfast", value: "Breakfast", color: "hsl(141, 95%, 90%)"}
      - { label: "", value: "", color: "hsl(77, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
      content_alignment: text-align-left
      content_vertical_alignment: align-top
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
    options:
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
      content_alignment: text-align-left
      content_vertical_alignment: align-top
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: true
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  source_data: query
  source_form_result: "WHERE notetype = \"recipe\""
  source_destination_path: Personal Shelf/Cookbook/Recipes
  row_templates_folder: Intel Shelf/zz_Templates
  current_row_template: 
  pagination_size: 50
  font_size: 16
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: true
  implementation: default
filters:
  enabled: false
  conditions:
```