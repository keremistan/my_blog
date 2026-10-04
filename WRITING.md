# Writing & Publishing Guide

Welcome to your Quartz 5 blog!

## Quick Workflow (How to Publish a Post)

To publish a new post, all you need to do is:

1. **Create a markdown file** in `content/posts/` (e.g. `content/posts/my-new-post.md`).
2. Add the frontmatter at the top:
   ```yaml
   ---
   title: My New Post Title
   date: 2026-10-04
   tags:
     - tech
     - thoughts
   description: A short summary of what this post is about.
   draft: false
   ---
   ```
3. Write your content in Markdown below the frontmatter.
4. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "Add new post: My New Post Title"
   git push origin v5
   ```
5. GitHub Actions will automatically build and deploy your site to GitHub Pages in ~1-2 minutes!

---

## Local Preview

Whenever you want to preview your changes before pushing:

```bash
npx quartz build --serve
```

Then open `http://localhost:8080` in your browser. It includes live-reloading as you save markdown files.

---

## Useful Features

- **Internal Links**: Link to another post using `[[posts/hello-world|Hello World]]` or standard markdown links `[Hello World](./hello-world)`.
- **Images**: Place image files in `content/` (e.g., `content/images/pic.png`) and reference them with `![alt text](images/pic.png)`.
- **Drafts**: Set `draft: true` in the frontmatter to keep writing without publishing it to the live site.
- **Tags**: Any tags listed under `tags` will automatically get their own tag index page.
