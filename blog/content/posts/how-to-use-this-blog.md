---
title: "How to Use This Hugo Blog Project"
date: 2025-06-25T12:00:00+08:00
draft: false
description: "A quick guide to writing and managing your technical blog with Hugo."
---

Welcome to your new Hugo-powered technical blog! This article will help you get started:

## 1. Writing Blog Posts in Markdown
- All your posts go in the `content/posts/` directory.
- Use the command:
  ```
hugo new posts/my-new-post.md
  ```
- Edit the generated Markdown file. Set `draft: false` in the front matter to publish.

## 2. Running the Local Server
- Start the server with:
  ```
hugo server -D
  ```
- Visit [http://localhost:1313](http://localhost:1313) to preview your site.

## 3. Customizing Your Site
- Edit `hugo.toml` for site settings.
- Change the theme or configure Ananke as you like.

## 4. Publishing
- Run `hugo` to generate the static site in the `public/` folder.
- Deploy the contents of `public/` to your web host or GitHub Pages.

Happy blogging!
