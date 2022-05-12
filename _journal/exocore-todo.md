---
layout: journal
category: journal
date: 2022-04-22
tags: meta exocore computers todo
---

# Exocore Production Log

# Features to consider for the exocore, and resources on them

## Plugin Lists
* [GitHub - planetjekyll/awesome-jekyll-plugins: A collection of awesome Jekyll plugins (gems, scripts, pasties, etc.)](https://github.com/planetjekyll/awesome-jekyll-plugins)
* [GitHub - planetjekyll/awesome-jekyll-editors: A collection of awesome Jekyll editors](https://github.com/planetjekyll/awesome-jekyll-editors)

## Online Composition and Editing
* [GitHub - netlify/netlify-cms: A Git-based CMS for Static Site Generators](https://github.com/netlify/netlify-cms)
* [GitHub - jekyll/jekyll-admin: A Jekyll plugin that provides users with a traditional CMS-style graphical interface to author content and administer Jekyll sites.](https://github.com/jekyll/jekyll-admin)
* [GitHub - prose/prose: A Content Editor for GitHub.](https://github.com/prose/prose)

## Graph Visualisation

![](/attachments/connection-graph.png)
{:.right}

* [GitHub - Zettelkasten-Method/zkviz: Zettel Network Visualizer](https://github.com/Zettelkasten-Method/zkviz/)
* [Post on Zettelkasten Graph Visualisation for Jekyll](https://forum.zettelkasten.de/discussion/102/static-website-hugo-jekyll-etc-as-a-zettelkasten)
* [Designing a Personal Knowledgebase – A Curious Mix](http://www.acuriousmix.com/2014/09/03/designing-a-personal-knowledgebase/)

## oEmbeds and Embeds for Tweets and PDFs 
* [GitHub - rob-murray/jekyll-twitter-plugin: A Liquid tag plugin for the Jekyll blogging engine that embeds Tweets, Timelines and more from Twitter API](https://github.com/rob-murray/jekyll-twitter-plugin)
* [jekyll_oembed](https://rubygems.org/gems/jekyll_oembed)
* [jekyll-pdf-embed ](https://rubygems.org/gems/jekyll-pdf-embed)
* [digital-garden-jekyll-template/embed_tweets.rb at master · maximevaillancourt/digital-garden-jekyll-template · GitHub](https://github.com/maximevaillancourt/digital-garden-jekyll-template/blob/master/_plugins/embed_tweets.rb)

## Backlinking and Visualisation of Note Connections
* [GitHub - manunamz/jekyll-namespaces: Add file.name.spacing support for jekyll.](https://github.com/manunamz/jekyll-namespaces)
* [GitHub - manunamz/jekyll-graph: Add graph(s) support for jekyll.](https://github.com/manunamz/jekyll-graph)
* 

## Snippets and Syntax Support for VSCode
* [Jekyll Snippets - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=ginfuru.vscode-jekyll-snippets)
* [jekyll-syntax-support](https://marketplace.visualstudio.com/items?itemName=ginfuru.ginfuru-vscode-jekyll-syntax)

## Misc
* [Octopress](http://octopress.org/)
* [GitHub - keithmifsud/jekyll-target-blank: Automatically opens external links in a new browser for Jekyll Pages, Posts and Docs.](https://github.com/keithmifsud/jekyll-target-blank)
* [GitHub - jekyll/jekyll-mentions: @mention support for your Jekyll site](https://github.com/jekyll/jekyll-mentions)
* [premonition](https://rubygems.org/gems/premonition)

---

## Other Features
- 'ID' YAML metadata tag for Wiki notes, to allow provision of both a title and an ID, rather than the ID being the title. Allows for independent manipulation of ID, and mnemonic titles. [Some info on identifiers in ZK](https://zettelkasten.de/posts/add-identity/)
- Addition of VSCode tags for identifiers to insert into template notes
- Citation management doubling as PDF storage/database [Manage Citations for a Zettelkasten • Zettelkasten Method](https://zettelkasten.de/posts/bibliography-zettelkasten/)
- Images should all link to themselves
- Need backlink graph visualisation — steal from [here?](https://github.com/maximevaillancourt/digital-garden-jekyll-template/tree/master/_plugins)
- FIX Netlify build error when invalid links
- Implement forelinks
- link somewhere to jekyll-wikilinks documentation
- edit image paste settings to be simplest possible — base image path, input box etc
- Pinned Notes:
  - Pinned: true/false in metadata
  - Pinned note appears in sidebar
- Github Actions daily push
- Build ~3 more themes 
- Use DOCKER
  - [Compile a Jekyll project without installing Jekyll or Ruby by using Docker](https://dev.to/michael/compile-a-jekyll-project-without-installing-jekyll-or-ruby-by-using-docker-4184)
  - [Docker Desktop for Mac user manual](https://docs.docker.com/desktop/mac/)
  - [Building and Deploying Jekyll Sites using Docker - Part Two - martinpeck.com](https://martinpeck.com/jekyll/blog/containers/2019/02/03/build-and-deploy-jekyll-with-docker-part2/)
- Clean up HEAD
- Github Actions: Push at a particular time — once a day 
  - [Events that trigger workflows - GitHub Docs](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows)


# TODO 
- Docker 
  - Learn how it works 
  - Can a docker image be altered later? or must the image be taken after all relevant changes have been made?
  - Craft a Docker image for the exocore
- Make graph work again
- Github actions setup
- Pinned note functionality
- ~3 more themes
- Clean up HEAD
- Clean up .config
- Clean up root directory
- Clean up warning messages
- Make all images link to self
- Make mobile compatible
- Clean gemfile of unused plugins
- Complete onboarding guide 
- Decide on best online CMS
  - Prose.io?
  - Jekyll CMS?
  - Other? See above
- Recipes section
- Books section
-  Writeups of every feature
-  Convert Exocore to purely instructional 
-  Jekyll Snippets for VSCode
-  VSCode Jekyll serve integration
-  Create Auto-push every 24hrs
   - [GitDoc?](https://marketplace.visualstudio.com/items?itemName=vsls-contrib.gitdoc)
   -  Github Actions
-  Make daily note delete if unused
-  Choose theme on front end — user chooses theme
-  Make exocore template repo
- Flesh out setup guide (with screenshots)
  - netlify one click setup
    - sign in with github
  - Git GUI / Cloning your repo
- Add comments feature