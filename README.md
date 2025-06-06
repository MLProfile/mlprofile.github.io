# MLProfile — Website

This repository hosts the website for **Profile**, a research initiative, built with [Jekyll](https://jekyllrb.com/) and deployed via [GitHub Pages](https://pages.github.com/) using the official **Cayman theme**.

Go [there](https://mlprofile.github.io/) to see the live site.
## Structure

This site is built with:
- **Markdown** for content (`.md` files)
- **MathJax** for LaTeX-style math rendering
- **Cayman** Jekyll theme (official GitHub Pages theme)
- **GitHub Actions** for automatic deployment

## Main Pages

- [`index.md`](index.md) — Home
- [`about.md`](about.md) — About the project
- [`publications.md`](publications.md) — Publications
- [`contact.md`](contact.md) — Contact information

## 🧮 Writing Math with LaTeX

MathJax is included for rendering math expressions.

- Inline math:  
  Write `\\( E = mc^2 \\)` → \\( E = mc^2 \\)

\\( E = mc^2 \\)

$$ 
E = mc^2 
$$

- Block math:  
  ```markdown
  $$
  \\int_0^\\infty e^{-x^2} dx = \\frac{\\sqrt{\\pi}}{2}
  $$
  ```
  
  $$
  \\int_0^\\infty e^{-x^2} dx = \\frac{\\sqrt{\\pi}}{2}
  $$

 \\(  \\int_0^\\infty e^{-x^2} dx = \\frac{\\sqrt{\\pi}}{2} \\)

## ➕ How to Add a New Page

To add a new page (e.g., a "Team" page):

1. Create a new Markdown file like `team.md` with a front matter block:

   ```markdown
   ---
   title: Team
   ---

   ## Our Team

   - Dr. Alice Smith
   - Prof. John Doe
   ```

2. Link to the new page from `index.md` or other pages:

   ```markdown
   [Home](index.md) | [Team](team.md)
   ```

3. Commit and push your changes (on main) — GitHub Pages will rebuild the site automatically.

## ⚙️ Configuration

To change the site’s title, description, or theme, edit [`_config.yml`](./_config.yml):

```yaml
title: Project X
description: Research project website
theme: jekyll-theme-cayman
```

## 🚀 Deployment

This site is automatically built and deployed by **GitHub Actions**.

No local installation of Ruby or Jekyll is required.

