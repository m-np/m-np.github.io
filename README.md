# mandarparab.github.io

Personal website for Mandar Parab — ML Engineer, AI Researcher.

## Deploy to GitHub Pages in 5 minutes

### 1. Create the repository
- Go to github.com and create a new repository named exactly: `mandarparab.github.io`
- Make it **public**
- Don't initialize with a README

### 2. Push the files
```bash
git init
git add index.html README.md
git commit -m "initial site"
git branch -M main
git remote add origin https://github.com/mandarparab/mandarparab.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages
- Go to your repo → Settings → Pages
- Source: "Deploy from a branch"
- Branch: `main` / `/ (root)`
- Save

Your site will be live at **https://mandarparab.github.io** within ~2 minutes.

---

## Add your photo

1. Create an `images/` folder in the repo
2. Add your photo as `images/profile.jpg`
3. In `index.html`, find this comment in the sidebar:
   ```html
   <!-- Replace with: <img src="images/profile.jpg" ...> -->
   ```
4. Replace the `<span class="avatar-initials">MP</span>` line with:
   ```html
   <img src="images/profile.jpg" alt="Mandar Parab" style="width:100%;height:100%;object-fit:cover;border-radius:50%;">
   ```

## Add more pages (Research, Writing, Projects)

Create separate HTML files using the same layout — copy `index.html`, update the `<main>` content, and update the nav `class="active"` to the correct link.

```
mandarparab.github.io/
├── index.html          ← homepage (this file)
├── research.html       ← detailed research page
├── writing.html        ← all articles and posts
├── projects.html       ← project details
└── images/
    └── profile.jpg     ← your photo
```

## Custom domain (optional)

If you buy `mandarparab.com`:
1. In repo root, create a file called `CNAME` containing just: `mandarparab.com`
2. In your domain registrar, add a CNAME record: `www` → `mandarparab.github.io`
3. In GitHub Pages settings, enter your custom domain

---

Built with plain HTML/CSS. No frameworks, no build step, no dependencies.
