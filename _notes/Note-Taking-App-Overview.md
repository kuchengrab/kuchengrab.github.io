---
title: Note-Taking App Overview
---

# Overview of Note-Taking Apps
list of markdown-based apps for personal knowledge management (PKM), with wiki and/or journaling and todo functions.

## shortlist
### dendron
- https://www.dendron.so/
-
  > *The hierarchical note taking tool that grows as you do!*
  *Dendron is an open-source, local-first, markdown-based, note-taking tool built on top of VSCode.*
- #opensource , #markdown , VScode, #zotero , #backlinks , #graph-view, #templates
- emphasises a good naming scheme for notes (continually adapt through "refactoring"), e.g. `book.hooks-bell-feminism-is-for-everybody.notes`
- for very advanced users/programmers (familiar with VScode)
  - but seems really advanced, thought-through and cool! 🤓
  - style can be adapted with CSS
  - nice publishing functionality
- most advanced open source tool, but considerable lerning curve


### zettlr
- https://zettlr.com/

  > *A Markdown Editor for the 21st century.*
- #markdown , #tags , #id #opensource , #zotero , #pandoc , ui #4/5
- (-) no backlinks, no graph view, no auto-suggest
  - zettlr doesn't use a database, therefore backlinks would have to be created for each note individually = slow, resource hungry
  - link = search
- zettelkasten with ID-pattern ("raw" in text)
- metadata with YAML (example)
    ```
    ---
    title: "Your document's title"
    keywords:
      - A keyword
      - Another keyword
    author:
      - The Zettlr Team
    ...
    ```
- (+) zettlr recognizes different kinds of tags, from YAML and hashtags
  - not compatible with nested tags
- (+) integration with pandoc & zotero (Better BibTeX references)

### obsidian
- https://obsidian.md/
  > *A second brain, for you, forever.*
  *Obsidian is a powerful knowledge base that works on top of a local folder of plain text Markdown files.*
- workspaces (notebooks), #tags , #graph-view , #backlinks , #proprietary
- optional: zettelkasten-id, journaling, `[[Wiki-Links]]` etc.
- sleek UI #5/5
- possible to use folders (which have no impact on internal links), support for nested tags (e.g. `Berlin/Alexanderplatz`) 
- judgement: looks very good, very functional. unfortunately not open source

## conceptually slightly different
### logseq
- https://logseq.com
  > *A privacy-first, open-source (frontend now, backend later) platform for knowledge sharing and management.*

![](media/upload_2fa11f9a1a386b21f8587357aada82c0.png)
- synchronization with github repository
- almost clone of *[roam research](https://md.zusammenkunft.berlin/#roam-research)* , #relational , #opensource , #graph-view #backlinks
- uses a database = changes in files are not automatically reflected in app, but [[backlinking]] is enabled
- very sleek UI
- every bullet point can be referenced or embedded
- limited #markdown (no headings), strange own #syntax with `#` at the beginning of each line (◦bullet point), representing indentation (example)
  ```
  ---
  title: Overview of Note-Taking Apps
  alias: Note Apps
  ---

  ##
  ## **logseq**
  ### https://logseq.com
  ### 
  > _A privacy-first, open-source (frontend now, backend later) platform for knowledge sharing and management._
  ### synchronization with github repository
  ```
	 
- cool concept, but not copatible with other tools, rather online-first than local-first


### joplin
- https://joplinapp.org/
  > *Joplin - an open source note taking and to-do application with synchronization capabilities for Windows, macOS, Linux, Android and iOS.*
- #markdown , #tags , #opensource
- very similar to Evernote, focus on synchronization with different devices
- cryptic format (note-id as filename, but acceptable export to proper #markdown )
  - ![](media/upload_b5514f721c2033503a24090e709b23d1.png)
  - metadata at the end of file (example)
      ```
      id: 3b3a9fb830894f889ce764ce47cf17c7
      parent_id: 3c6f7e9b98e24ac4ac473a33105a2374
      created_time: 2020-11-26T17:11:29.759Z
      updated_time: 2020-11-26T18:58:55.638Z
      is_conflict: 0
      latitude: 0.00000000
      longitude: 0.00000000
      altitude: 0.0000
      author: 
      source_url: 
      is_todo: 0
      todo_due: 0
      todo_completed: 0
      source: joplin-desktop
      source_application: net.cozic.joplin-desktop
      application_data: 
      order: 1602180058164.625
      user_created_time: 2020-11-26T17:11:29.759Z
      user_updated_time: 2020-11-26T18:58:55.638Z
      encryption_cipher_text: 
      encryption_applied: 0
      markup_language: 1
      is_shared: 0
      type_: 1
      ```


## notable mentions

### notable
- https://notable.app/ -- https://github.com/notable/notable
  > *The Markdown-based note-taking app that doesn't suck.*
- #hierarchical (notebooks --> tags --> sub-tags)
- #markdown , #tags , #tags-nestable , #YAML , #html elements
- cool features: Multi-Note Editor, nested tags (but not compatible)
  - (-) no auto-suggest of tags
- metadata and tags with #YAML , example:
    ```
    ---
    tags: [français, urban/housing]
    title: Les luttes de logement en europe
    created: '2021-04-17T22:51:24.274Z'
    modified: '2021-04-26T14:48:14.187Z'
    ---
    ```
- ±compatible with **zettlr**
- judgement: cool minimalist app with some good ideas, but not completely mature yet

### roam research
- https://roamresearch.com/
  > *A note-taking tool for networked thought.*
- --> completely #relational, #proprietary, #graph-view, #backlinks
- super expensive, "what everyone is talking about" ... just for reference

### trilium
- https://github.com/zadam/trilium
  > *Trilium Notes is a hierarchical note taking application with focus on building large personal knowledge bases.*
- (-) uses #wysiwyg (#html) instead of markdown
- #hierarchical note organisation as well as #graph-view and #backlinks
- UI is alright – 3/5
- judgement: no markdown = dealbreaker

### marktext
- https://marktext.app/ | https://github.com/marktext/marktext
  > *Simple and Elegant Markdown Editor, focused on speed and usability.* 
- #opensource, Linux, MacOS, Windows
- markdown editor for focused writing


### typora
- https://typora.io/
- > *a truly minimalist markdown editor – real live preview* 
- #proprietary #markdown 
- focused writing

