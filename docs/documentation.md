# Personal Hugo Site - Workflow Documentation

This document outlines the basic workflow for maintaining and updating the website at [hafeezulrzq.github.io](https://hafeezulrzq.github.io).

---

## 1. Making Changes

Whenever you make any changes (e.g., to config, layouts, pages):

- **Build the site locally** by running:

  ```bash
  hugo
  ```

  > This generates the latest static files inside the `/public` folder.

- **Preview the site locally** to check your changes:

  ```bash
  hugo server -D
  ```

  > This will launch a live server (usually at `http://localhost:1313`) and automatically reload on changes.

---

## 2. Adding New Blogs or Projects

When creating new content:

- Create a new blog post:

  ```bash
  hugo new blogs/my-new-blog.md
  ```

- Create a new project entry:

  ```bash
  hugo new projects/my-new-project.md
  ```

- Edit the newly created `.md` file inside `content/blogs/` or `content/projects/` accordingly.

**Reminder:**  
Each post usually requires setting:
- `title`
- `date`
- `summary`
- `tags`
- `draft: true/false`
- `cover image` (optional)

---

## 3. Adding Images

- Store your images at:

  ```
  docs/images/
  ```

- Reference them in your Markdown files like:

  ```markdown
  ![Alt text](/docs/images/your-image.png)
  ```

---

## 4. Deployment

After finalizing your changes:

- Run:

  ```bash
  hugo
  ```

- Commit and push the **updated `/public` folder** (if you're pushing manually), or if using GitHub Pages:
  - Make sure your `hugo` output (`public/`) is set to the correct branch (usually `main` or `docs` branch depending on your settings).

---

## 5. Other Tips

- If you have posts still being drafted (`draft: true`), they will **not** show unless you run `hugo server -D`.
- Always double-check image links — wrong paths can cause broken images on GitHub Pages.
- Keep the file naming consistent and lowercase to avoid issues on different servers (e.g., `my-blog.md`, not `My Blog.md`).
- If you install a new theme or update theme settings, run:

  ```bash
  hugo mod tidy
  ```

- To update `hugo` to the latest version:

  ```bash
  brew upgrade hugo
  ```

  (if you installed via Homebrew on Mac)

---

# 📋 Quick Command Summary

| Purpose               | Command                    |
|------------------------|-----------------------------|
| Build site             | `hugo`                     |
| Preview site locally   | `hugo server -D`            |
| New blog post          | `hugo new blogs/title.md`   |
| New project entry      | `hugo new projects/title.md`|

