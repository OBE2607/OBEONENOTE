---

database-plugin: basic

---
# 001MATERIEL_CLI

```yaml:dbfolder
name: SUIVI MATERIEL
description: SUIVI MATERIEL
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
    isHidden: true
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
  Selectionj:
    input: select
    accessorKey: Selectionj
    key: Selectionj
    id: Selectionj
    label: Selectionj
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: 1
    isSorted: true
    isSortedDesc: false
    options:
      - { label: "Logiciel", value: "Logiciel", color: "hsl(39, 95%, 90%)"}
      - { label: "Matériel", value: "Matériel", color: "hsl(73, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  ENTREPRISE:
    input: relation
    accessorKey: ENTREPRISE
    key: ENTREPRISE
    id: ENTREPRISE
    label: ENTREPRISE
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 200
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: 002DBFLODER/000PROJET/001PROJET.md
      relation_color: hsl(256,41%,32%)
      wrap_content: true
  SITE01:
    input: text
    accessorKey: SITE01
    key: SITE01
    id: SITE01
    label: SITE01
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 79
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  SITE02:
    input: text
    accessorKey: SITE02
    key: SITE02
    id: SITE02
    label: SITE02
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 51
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  SITE03:
    input: text
    accessorKey: SITE03
    key: SITE03
    id: SITE03
    label: SITE03
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 70
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  SITE04:
    input: text
    accessorKey: SITE04
    key: SITE04
    id: SITE04
    label: SITE04
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 37
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  SITE05:
    input: text
    accessorKey: SITE05
    key: SITE05
    id: SITE05
    label: SITE05
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 40
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  SITE06:
    input: text
    accessorKey: SITE06
    key: SITE06
    id: SITE06
    label: SITE06
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 15
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Nbrs:
    input: text
    accessorKey: Nbrs
    key: Nbrs
    id: Nbrs
    label: Nbrs
    position: 12
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
  REF:
    input: relation
    accessorKey: REF
    key: REF
    id: REF
    label: REF
    position: 10
    skipPersist: false
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
      related_note_path: 002DBFLODER/001MATERIEL_TYPE/001MATERIEL_TYPE.md
      relation_color: hsl(247,72%,53%)
  MATERIEL:
    input: rollup
    accessorKey: MATERIEL
    key: MATERIEL
    id: MATERIEL
    label: MATERIEL
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 51
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      asociated_relation_id: REF
      rollup_action: Original Value
      rollup_key: REFERENCE
  MATERIEL_RECUT:
    input: select
    accessorKey: MATERIEL_RECUT
    key: MATERIEL_RECUT
    id: MATERIEL_RECUT
    label: MATÉRIEL REÇUT
    position: 13
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "oui", value: "oui", color: "hsl(65, 95%, 90%)"}
      - { label: "non", value: "non", color: "hsl(23, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  MATERIEL_ENVOYE:
    input: select
    accessorKey: MATERIEL_ENVOYE
    key: MATERIEL_ENVOYE
    id: MATERIEL_ENVOYE
    label: MATÉRIEL ENVOYE
    position: 15
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "oui", value: "oui", color: "hsl(137, 95%, 90%)"}
      - { label: "non", value: "non", color: "hsl(125, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  DATE_MATERIEL_ENVOYE:
    input: calendar
    accessorKey: DATE_MATERIEL_ENVOYE
    key: DATE_MATERIEL_ENVOYE
    id: DATE_MATERIEL_ENVOYE
    label: DATE_MATERIEL_ENVOYE
    position: 16
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
  LIEU_RECEPTION:
    input: text
    accessorKey: LIEU_RECEPTION
    key: LIEU_RECEPTION
    id: LIEU_RECEPTION
    label: LIEU DE RECEPTION
    position: 17
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
  DATE_RECEPTION:
    input: calendar
    accessorKey: DATE_RECEPTION
    key: DATE_RECEPTION
    id: DATE_RECEPTION
    label: DATE_RECEPTION
    position: 14
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
config:
  remove_field_when_delete_column: false
  cell_size: wide
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 10
  font_size: 13
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: dd-MM-yyyy
  datetime_format: "dd-MM-yyyy HH:mm:ss"
  metadata_date_format: "dd-MM-yyyy HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: false
  conditions:
      - condition: AND
        disabled: false
        label: "G REGUILLON"
        color: "hsl(242,75%,50%)"
        filters:
        - field: ENTREPRISE
          operator: CONTAINS
          value: "GROUPE_REGUILLON"
          type: relation
```