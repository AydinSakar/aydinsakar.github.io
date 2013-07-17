---
layout: post
title: "Octopress"
date: 2013-07-17 11:50
comments: true
categories: 
- Octopress
- GitHub
- Tools
---

I am using [Octopress](http://octopress.org/) to publish this blog.

I am using Windows 7 for daily work so had to install Octopress and GitHub on a Windows machine. I am planning to write a series of tutorials on the problems I faced making all work together with Windows.

I just want to make a brief note about the confusion I had when I tried to understand Octopress: The repository structure.

You have to have username.github.io named repository at [GitHub](https://github.com/) to use GitHub Pages. The repository of this blog is: [aydinsakar.github.io](https://github.com/AydinSakar/aydinsakar.github.io) You can also have project pages, but that is another topic for a blog post.

Octopress manages two branches in your username.github.io repository:

1. master branch:
This is the actual branch that GitHub uses to publish your blog. When Github sees a push to this branch, they republish your content.
2. source branch:
This contains the source of Octopress *AND* your blog posts. Octopress generates the content from this branch and puts everything in a "_deploy" directory which is the actual "master" branch which is then pushed to GitHub. You have to remember to commit and push the "source" branch yourself.

The bottom line is "master" is the generated blog, and the "source" is the raw stuff. They are not actually branches of a source tree in a usual sense. These two branches are completely different thigs which you should never manually deal with. This is kind of a *hack* that I had to understand, and which probably was the source of quite a bit of a confusion.