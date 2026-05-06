---
title: "Hello World: Why I finally started this blog"
date: 2026-05-05T12:40:46-03:00
draft: false
---

One day, while eating burgers with friends, the conversation drifted toward technology (it happens more often than we admit!). I met someone who was struggling to learn **design patterns**. I tried explaining one in just a few minutes—I’ve always loved seeing the world through an **object-oriented lens** and finding ways to simplify complex topics.

When she asked if I had a post she could read, all I had was an old PowerPoint presentation. 

That moment reminded me why I always wanted a blog. I love sharing knowledge; it makes me feel useful to help others bridge that gap between "this is complicated" and "oh, I get it now!"

## Why Hugo?

I initially planned to build this with **React** (since that's where my skills are), but I realized the most important part of a blog is the *content*, not the dev time. I wanted something fast, efficient, and Markdown-based. 

Enter **[Hugo](https://gohugo.io/)**: a static site generator that let me focus on writing rather than boilerplate. I tweaked a theme I liked, set up GitHub Actions, and now this post is **fresh out of the oven**.

---

## Quick Start: How I set this up

If you're looking to start your own, here’s the high-level roadmap:

### Install Hugo

Follow the [official documentation](https://gohugo.io/installation/) for your specific OS.

### Pick a Theme

Once you find a [theme](https://themes.gohugo.io/) you love, add it as a submodule:

```bash
git submodule add https://github.com/theNewDynamic/<theme>.git themes/<theme>
```

### Set Configurations & Content

**Config:** Every setting you need (title, theme, social links) is in the `hugo.toml` file.

**New Post:** To create a draft, use the command: `hugo new content posts/my-first-post.md`.

**Local Preview:** Run `hugo server -D` to see your changes locally before pushing.

### Deploy with GitHub Pages

I used **GitHub Actions** for automation. You need to create a workflow file at `.github/workflows/hugo.yaml` with the build steps. Then:

Push your code to the `main` branch.

In your repository settings, go to **Settings > Pages**.

Select `GitHub Actions` as the **Source**.

You can take a look at my [blog repository](https://github.com/AlyStrat/alystrat.github.io/blob/main/.github/workflows/hugo.yaml) for the exact workflow configuration.

### Some useful links:

- [Hugo Documentation](https://gohugo.io/)
- [Hugo Themes](https://themes.gohugo.io/)
- [GitHub Actions for Hugo](https://gohugo.io/host-and-deploy/host-on-github-pages/)

> Updated: 2026-05-05

That's all folks!
