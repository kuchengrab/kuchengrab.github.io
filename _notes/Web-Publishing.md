---
title: Web-Publishing
---

- What is the purpose? 
    - Is it a (rather) linear book, hierarchically organised in chapters and subchapters?
    - Is it a collection of notes, connected to each other (wiki)?

- Who should be able to edit/view it?
    - Only you?
    - You and sometimes others?
    - A whole team collaborating on content creation?    

## Wiki - Without Own Server Infrastructure/Self-Hosting
- GitHub
    - create a new (public) [[repository|Git]], use the wiki tab
    - clone it to your local device (`https://github.com/user/repository-name.wiki.git`)
    - make sure to use only links that GitHub Wiki understands
        - like `[[Page Name]]` pointing to `Page-Name.md`
        - `[[link text|Page Name]]` like `[[shortlist|Note-Taking-App-Overview#shortlist]]` for [[shortlist|Note-Taking-App-Overview#shortlist]]
        - or Markdown links `[like this](https://github.com/kuchengrab/md-publishing/wiki)`
    - edit directly in [[VSCode, Zettlr or Obsidian|Note-Taking-App-Overview#shortlist]], push to GitHub Wiki repository

- [TiddlyWiki](https://tiddlywiki.com/)
    - can [easily be shared](https://tiddlywiki.com/#Sharing%20your%20tiddlers%20with%20others) using a shared folder
- [[logseq|Note-Taking-App-Overview#logseq]] using github repository


## Native Self-Hostable Wiki Apps
- [Wiki.js](https://js.wiki/)
- [django-wiki](https://github.com/django-wiki/django-wiki)
- [gollum Wiki](https://github.com/gollum/gollum/wiki)

## Book-Like Apps
- GitBook
- [BookStack](https://www.bookstackapp.com/)

## Static Website Generator
- using GitHub Pages / [GitLab Pages](https://about.gitlab.com/stages-devops-lifecycle/pages/)
- \+ static website generator
    - Jekyll
        - [digital-garden-jekyll-template](https://github.com/maximevaillancourt/digital-garden-jekyll-template)
        - [simply-jekyll Theme](https://simply-jekyll.netlify.app/posts/introduction-to-simply-jekyll)
        - [just-the-docs](https://github.com/pmarsceill/just-the-docs)
    - Middleman, Hexo, Hugo, Pelican

## References
https://nesslabs.com/digital-garden-set-up

[Dendron: Publishing](https://wiki.dendron.so/notes/579e379b-3eca-4676-b51c-c66eb26a11b8.html)