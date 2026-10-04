# Kerem Dede's Blog

A personal blog built with Quartz 5 and hosted on GitHub Pages.

## Writing & Publishing

To create a new post:
1. Add a Markdown file in `content/posts/` (e.g. `content/posts/my-post.md`).
2. Add your post frontmatter:
   ```yaml
   ---
   title: My Post Title
   date: 2026-10-04
   tags:
     - tech
   description: Brief summary
   ---
   ```
3. Commit and push:
   ```bash
   git add .
   git commit -m "Add new post"
   git push
   ```

GitHub Actions automatically builds and publishes your site to GitHub Pages.

For more details, see [WRITING.md](WRITING.md).

## Local Preview

```bash
npx quartz build --serve
```
View at `http://localhost:8080`.
