---
published: false
title: "Publish blog posts from GIT to dev.to"
cover_image: "https://user-images.githubusercontent.com/10644132/124338461-f7744b00-db5c-11eb-8047-eb073cc632f3.png"
description: "Automate publishing your article from git markdown to dev"
tags: devto,publication,continuousdeployment
series:
canonical_url: ""
---

<div align="center">

[![Actions Status](https://github.com/anilkulkarni87/dev.to/workflows/CI/badge.svg)](https://github.com/anilkulkarni87/dev.to/actions)

</div>

# Publish blog posts from GITHUB to dev.to

This is a template repo which where I am testing and building solution for automated publishing of my articles/blog posts to dev. It's just a lot of work to post the same article across places and hence I decided to automate publishing my posts to dev and eventually any other personal blogs.

Dev exposes API through which you could do a lot of things. I am currently only creating articles which will be in your drafts. 

![image](https://user-images.githubusercontent.com/10644132/124338461-f7744b00-db5c-11eb-8047-eb073cc632f3.png)


## Approach
- Clone this repo, cleanup the files and arrange your blog posts.
- Create a markdown file for your blog post. You can check the folder structure in the repo.
- Setup your DEV TOKEN in your repo with the name as `GIT_TO_DEV`
- Commit the changes made to your .md files.
- Voila after the workflow is complete, you can see the blog posts created in draft. 
- Also, I am persisting the json payload of the article with the id populated.

### Next steps
- Identify new files and modified markdown files
- For new files, create new articles
- For modified, update the articles
    - Read the json and call the Update api


### Thanks
- [Ana María Martínez Gómez](https://github.com/Ana06/get-changed-files) - Tracking changed files
- [Stefan Zweifel](https://github.com/stefanzweifel/git-auto-commit-action) - Committing the changes file from a workflow
- [Maxime](https://dev.to/maxime1992/manage-your-dev-to-blog-posts-from-a-git-repo-and-use-continuous-deployment-to-auto-publish-update-them-143j) - For the triggering a thought
- [Chris Amico](https://github.com/eyeseast/python-frontmatter) - For parsing front matter from Markdown file

### Bugs/Changes
Please modify any typos or corrections and create a pull request to make this better.
