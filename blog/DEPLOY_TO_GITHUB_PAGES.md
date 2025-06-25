# Deploying Your Hugo Blog to GitHub Pages

This guide explains how to publish your Hugo blog on GitHub Pages.

## 1. Build Your Site

In your `blog` directory, run:

```
hugo
```

This generates static files in the `public/` folder.

## 2. Create a GitHub Repository

- Go to GitHub and create a new repository (e.g., `yourusername.github.io` for a user site, or any name for a project site).

## 3. Push the `public/` Folder to GitHub Pages

### Option 1: Deploy to `gh-pages` Branch

1. In your `blog` directory, initialize a new git repo in `public/`:
   ```
   cd public
   git init
   git remote add origin https://github.com/yourusername/yourrepo.git
   git checkout -b gh-pages
   git add .
   git commit -m "Deploy Hugo site"
   git push -f origin gh-pages
   ```
2. On GitHub, set Pages source to the `gh-pages` branch.

### Option 2: Deploy to `docs/` Folder (for project pages)
- Move the contents of `public/` to a `docs/` folder in your main branch and set GitHub Pages source to `/docs`.

## 4. Configure `baseURL`
- In `hugo.toml`, set:
  ```
  baseURL = 'https://yourusername.github.io/'
  ```
  (or your custom domain)

## 5. Automate with GitHub Actions (Optional)
- You can automate deployment with a GitHub Actions workflow. See the Hugo docs for details: https://gohugo.io/hosting-and-deployment/hosting-on-github/

---

Now your blog will be live on GitHub Pages!
