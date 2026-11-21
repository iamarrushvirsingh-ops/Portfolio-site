# Arrush Vir Singh: Portfolio

My personal portfolio website. I'm a cybersecurity student at AKGEC, Ghaziabad, looking for SOC, VAPT and entry-level security roles.

The whole site is one file, `index.html`. It has no backend (no server code, no database), so it can be hosted for free on GitHub Pages or Vercel.

> Built with AI assistance (vibe coding). I planned it, steered the build and tested it.

---

## What's on the site

| Section | What it shows |
|---|---|
| **The room** | An animated pixel-art room. Clicking an object (laptop, terminal, pinboard, trophies, drums...) jumps to that part of the site. The drum kit plays a beat. |
| **Intro** | My name over a "paint" effect that swirls when you move your cursor. |
| **Work** | My projects (AI recon agent, OceanEmbed, Complaint Hub, PreClass), each with its own animated picture. |
| **Experience** | My internships and roles, as cards on a daytime-sky background. |
| **Skills** | A terminal that works (type `help` and press Enter) and skill-level meters. |
| **Achievements** | Game-style badges for training, education and what I'm learning next. |
| **About me** | My photo, a short bio and drum pads you can play. |
| **Contact** | Email (with a copy button), LinkedIn, GitHub and resume. |

Everything is drawn with code: there are no image files except my photo.

---

## Folder layout

```
portfolio-site/
├── index.html      ← the whole website
├── resume.pdf      ← my resume (add this yourself)
├── README.md       ← this file
└── assets/
    └── photo.jpg   ← my photo (add this yourself)
```

### Adding my photo
1. Pick a portrait photo, roughly 4:5 in shape (a bit taller than it is wide).
2. Name it exactly `photo.jpg`, all lowercase.
3. Put it inside the `assets` folder.

If the photo is missing, the site shows my pixel character instead, so nothing breaks.

### Adding my resume
1. Export the resume as a PDF.
2. Name it exactly `resume.pdf`, all lowercase.
3. Put it next to `index.html`, not inside `assets`.

Both Resume buttons on the site open this file. To update the resume later, replace the file and keep the same name.

### Changing text
All the words on the site are inside `index.html`. Open it in any text editor (VS Code, Notepad, gedit), search for the sentence you want to change with Ctrl+F, edit it and save.

---

## Viewing it on my own computer

- **Easiest:** double-click `index.html` and it opens in your browser.
- **Closer to the real thing:** open a terminal in the `portfolio-site` folder and run:
  ```bash
  python3 -m http.server 8000
  ```
  Then go to <http://localhost:8000> in the browser. Press Ctrl+C in the terminal to stop it.

---

## Putting it online

### Option A: GitHub Pages (recommended)

The site will live at **https://iamarrushvirsingh-ops.github.io**

1. Sign in to GitHub and click **New repository** (the green **New** button, or the **+** at the top right).
2. Name the repository exactly: `iamarrushvirsingh-ops.github.io`
3. Set it to **Public** and click **Create repository**.
4. On the new repository page, click **uploading an existing file**.
5. Drag in `index.html`, `README.md`, the `assets` folder and `resume.pdf` (if you have it). Drop the files themselves, not the `portfolio-site` folder that holds them.
6. Click **Commit changes** (this means "save").
7. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, set the branch to **main** and the folder to **/ (root)**, then click **Save**.
8. Wait 1–2 minutes, then open **https://iamarrushvirsingh-ops.github.io**

**Updating later:** in the repository, click **Add file → Upload files**, drag in the changed file (it replaces the old one), and click **Commit changes**. The live site updates in a minute or two.

### Option B: Vercel

The site will live at something like **https://arrush-portfolio.vercel.app**

1. First, put the files in a GitHub repository (steps 1–6 above; for Vercel the repository can have any name, for example `portfolio`).
2. Go to <https://vercel.com> and click **Sign Up → Continue with GitHub**. Choose the free **Hobby** plan.
3. Click **Add New… → Project**.
4. Find your repository in the list and click **Import**. If it isn't listed, click **Adjust GitHub App Permissions** and give Vercel access to it.
5. Set **Framework Preset** to **Other**. Leave the build settings empty, since there is nothing to build.
6. Click **Deploy**. When it's done, Vercel shows your live link.
7. Optional: to change the address, go to **Project → Settings → Domains** and edit the `.vercel.app` name, for example `arrush-portfolio.vercel.app`.

**Updating later:** upload the changed file to the GitHub repository and commit it. Vercel notices the change and redeploys by itself within about a minute.

---

## Notes

- **Turning off the effects:** the paint effect can be switched off from the **Menu**. If someone's device is set to reduce motion, the animations stay still automatically.
- **Sound:** the drums only make sound after someone clicks something, because browsers block sound until then.
- **Fonts:** Pixelify Sans, Archivo and JetBrains Mono, loaded from Google Fonts.

© 2026 Arrush Vir Singh
