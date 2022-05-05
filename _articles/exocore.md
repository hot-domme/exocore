---
layout: article
category: article
subtitle:
topic: Computers
date: 27 jan 2021
tags: exocore remilia computers web
---

# The Exocore Package

![](/attachments/exocore.png)

## Executive Summary

The exocore comprises a set of a few programs and plugins, rolling them into a package which can be customised infinitely and modularly; without any technical knowledge it can still be made your own, and with even a touch of technical knowledge (particularly CSS or HTML facility) it can be made into anything at all.

Its online component is a scaffolding for a website, and its offline component (fully functional without the online) is a filing system for knowledge, written output, or other data. Out of the box, it's a local directory of folders and interacting files forming an empty template for a [zettelkasten](https://zettelkasten.de/introduction/)/wiki, a platform for longform articles, a library of documents, a gallery of images, and an automatically created daily note. Mix and match these features as you wish; they are fully modular and independent.

in future, these exocores can comprise a webring linked by automatically updated network pages, as well as a [realtime IRC](https://xcela.org/#realtime-communicaiton) embed that connects all exocores to a chat server. They can also feature things like an automatically updated 'latest posts' feed from all other (or selected) exocores, or just 'related posts' (by [metadata](https://jekyllrb.com/docs/front-matter/) tags) from your own site.

As mentioned, a user would be free to use or not use any of these features, so if they want to create a self-hosted platform like substack with no extra features, this is facilitated.

### User experience:

A user will download the package in the form of a forked github repository, which will live on their local machine as a directory that can be manually or automatically pushed (synced) via [git](https://git-scm.com) to a website, which will merely represent the documents in the directory after they are processed into an HTML website.

A user can get by just fine only interacting with simple plaintext [markdown](https://www.markdownguide.org) files, and can write articles, notes, or any other written output in easily-learned markdown format. The are able to specify an optionally infinite number of variables for each document in a small human-readable metadata section at the top of the file: tags, title, subtitle, categories, layouts…

![](/attachments/girl-online.png){:.right}

The documents can then be differentially treated in the production of the site, or automatically arranged and categorised: for instance, a fully-developed article might appear on the website with a different layout template than a ZK note, and each ZK note might include a side-panel showing all the notes which reference it. The first [top-level markdown heading](https://www.markdownguide.org/basic-syntax#headings) of a note is taken to form the title of a note if none is specified in the metadata, and if no headings exist, the date of the note's creation or an incremented identifier number can be used.

Locally, the directory of notes (which will also be a git repository if you wish to publish as a website online) will be managed and maintained through a fork of [Foam](https://foambubble.github.io/foam/), an open source replication of a Roam Research-style notetaking system. The Foam fork arrives to the user as a package of two things:

- A template directory including markdown templates for simple creation of new markdown documents of different kinds (blogpost, journal entry, note, daily dump etc.), each treated differently in the rendering of your website.

- A set of [VS Code](https://code.visualstudio.com) plugins which allows the user to manage their notes directory through VS Code, facilitating easy linking between notes, URL management, and many other features. The directory can be easily hosted for free with [Netlify](https://www.netlify.com) or [Github Pages](https://pages.github.com). For easy hosting, Netlify is recommended— Github Pages uses a list of whitelisted plugins, and all others are disabled by default; to save the hassle of subverting this, use Netlify.



### Jekyll
***SUBJECT TO CHANGE:*** It is also recommended that a user set up their foam repository as a [Jekyll](https://jekyllrb.com) website repository so that they can preview how their website looks locally. Jekyll is a program which builds the site from your markdown files, and manages the relationships between the files, processes them according to their metadata, etc. 


### Customisability

The stack is an open-source repo and a suite of open-source programs and plugins, and is therefore ultimately customisable. The level of customisability depends only on your technical know-how, but minimal learnings yield compounding rewards. Here is an idea of the levels of control over your final website yielded by advancing levels of technical knowledge:

- **No technical knowledge:**
  - You can choose implement all of the above, and choose from a set of .CSS templates for your website to adjust its aesthetics. You can create articles, use the daily note functionality, store documents to the Library, create ZK notes and links between them, use backlinking and all other out-of-the-box features. Without technical knowledge all of the features listed [below](#features-out-of-the-box) are fully functional, and metadata customisability is still available. You should become acquainted with markdown syntax, but this is easy enough to guess at, or to learn in under half an hour. 

    For publishing, a very cursory knowledge of git will come in handy, but git has a helpful GUI, and Exocore documentation will include guides on how to publish your site.
  
- **HTML and CSS**
  - You will be able to edit included stylesheets and HTML templates to create a site which looks absolutely any way that you wish. Both thse languages are simple to learn, and even without learning them comprehensively a user can edit the provided templates and stylesheets to make major changes.  

- **Jekyll/Liquid**
  - You will be able to create logic functions to manipulate metadata stored in the markdown front matter, create custom menus or boxes with automatically generated content based on the front matter, assign your own front matter variables, and more. 

- **Ruby**
  - Learning Ruby is not at all necessary, but familiarity with it will facilitate you in packaging themes you have created for your exocore as Ruby Gems in case you would like to publish them for use by others. If you want to proliferate your particular model of the exocore, this is an easy way to package it.


## Full Tech Stack (Subject to additions)

- [Foam](https://foambubble.github.io/foam/) fork
- [VS Code](https://code.visualstudio.com) (and plugin package)
- [Git](https://git-scm.com) (For publishing)
- [Jekyll](https://jekyllrb.com) (optional, but recommended)
  
    Jekyll dependencies:
  - [Ruby](https://www.ruby-lang.org/en/)
  - [RubyGems](https://guides.rubygems.org/rubygems-basics/)
  - Others, included in Jekyll package


## Features Out of the Box:

### Daily
**Daily surf dumps**
- Created daily automatically, titled by the day
- Theme: Gemini
- Tags, next/prev, side/margin notes.
  
### Journal
**Longform, blog**
- Theme: Gwern
- Index: Chronological.
- Secondary: tags.
- Anchors, backlinks (at end), tags, hover, next/prev.
- Related posts, sidenotes, margin notes, comments, webmentions
- Secondary: TOC (dropdown)
- footnotes/sections

### Articles
**Full articles**
- Theme: Edith
- Index: Categorical.
- Secondary: tags.
- Anchors, backlinks (at end), tags, hover, next/prev, related posts, margin notes, comments
- Table of contents, sections, sectioned footnotes
- Webmentions
- sidenotes (== sectioned footnotes)

### Wiki
**Zettalkasten**
- Theme: Yotsuba
- Index: Graph node.
- Secondary: tags.
- Anchors, backlinks (at top), tags, hover, footnotes, next/prev.
- Side/margin notes (== Footnotes/asides), sections, comments, webmentions, related



[[business-virtue]]

[//begin]: # "Autogenerated link references for markdown compatibility"
[business-virtue]: ../_journal/business-virtue "The American Samurai"
[//end]: # "Autogenerated link references"