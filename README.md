# Ravi.me content

This repository contains the published site's posts and attachments.

- Put Markdown files directly in `posts/`, one file per post.
- Upload images and other media to `attachments/`.
- In a post, link to media with a path such as `![Alt text](../attachments/photo.jpg)`.
- Commit to `main` to publish. The workflow requests a website rebuild.

Each post can start with front matter:

```markdown
---
title: "My Post"
date: "2026-10-06"
description: "A short summary"
slug: "my-post"
---

Post content in Markdown.
```

To enable automatic rebuilds, add a fine-grained personal access token as the
`WEBSITE_REPO_TOKEN` Actions secret. Limit it to `solielkeisen/Ravi.me` and grant
**Contents: read and write** permission. The token is used only to send a
`repository_dispatch` event to the website repository.
