---
title: "Testing Giscus Comments"
date: 2024-05-20T00:59:47Z
author: "aefly"
slug: testing-giscus-comments
tags: ["Giscus", "Comments", "Testing"]
comments: true
draft: false
showToc: true
TocOpen: false
hidemeta: false
disableHLJS: false
hideSummary: false
searchHidden: false
ShowReadingTime: true
ShowBreadCrumbs: true
ShowCodeCopyButtons: true
ShowWordCount: true
ShowRssButtonInSectionTermList: true
UseHugoToc: true
---

## Introduction

For those who might not be familiar, [Giscus](https://giscus.app/) is an open-source, GitHub-powered comment system that allows you to embed GitHub discussions directly into your website.

## Why Giscus?

Let’s talk about why I chose Giscus for my blog. Traditional comment systems often come with privacy concerns and require maintaining separate user accounts. Giscus leverages GitHub’s infrastructure, which means it benefits from GitHub’s robust security, widespread use, and community engagement. Plus, it’s open-source, aligning with my values of transparency and community collaboration.

## Implementing Giscus

Integrating Giscus into my blog was pretty simple. Here’s the code snippet I used, which was generated directly with [giscus.app](https://giscus.app/):

```html
<script
 src="https://giscus.app/client.js"
 data-repo="aefly/blog"
 data-repo-id="R_kgDOL74QFg"
 data-category="Announcements"
 data-category-id="DIC_kwDOL74QFs4CfdDC"
 data-mapping="title"
 data-strict="0"
 data-reactions-enabled="1"
 data-emit-metadata="0"
 data-input-position="bottom"
 data-theme="dark_protanopia"
 data-lang="en"
 data-loading="lazy"
 crossorigin="anonymous"
 async
></script>
```

Then, with this snippet, I just needed to add it to `/layout/partials/comments.html`.

## Customizing Giscus

One of the great things about Giscus is its flexibility. You can customize various aspects, such as themes, languages, and positioning, to match your blog’s style and requirements. The script’s attributes are easy to modify, making it simple to tweak settings as needed.

## Testing the Setup

After adding the script to my blog, I tested it by navigating to this blog post and leaving a comment. If everything is working correctly, you should see the comment displayed below.

## Conclusion

Integrating Giscus into my blog has been great. It offers a modern, secure, and user-friendly way to manage comments using GitHub’s community. If you need a new comment system for your website, I highly recommend trying Giscus.

Feel free to leave a comment below with the new Giscus system. I look forward to your thoughts and feedback!
