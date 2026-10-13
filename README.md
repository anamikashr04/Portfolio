# The Threshold: how to publish on Vercel

This folder is the finished website. It is plain HTML, CSS and JavaScript, so there is **nothing to build, install or configure**. Vercel only needs to host the files.

## Option A: drag and drop (easiest, no accounts besides Vercel)
1. Unzip this file. You get a folder containing `index.html`.
2. Go to https://vercel.com and sign up or log in (free "Hobby" plan is fine).
3. Install the Vercel tool once: open Terminal (Mac) or Command Prompt (Windows) and run `npm i -g vercel`. This needs Node.js from https://nodejs.org.
4. In Terminal, go into the unzipped folder: `cd path/to/the/folder`
5. Run `vercel --prod`. Log in if asked. Press Enter to accept every question (project name can be anything, e.g. `anamika-portfolio`; if asked for a build command or output directory, leave them blank).
6. Vercel prints your live address (ends in `.vercel.app`). Open it and click through the site.

## Option B: through GitHub (no Terminal commands except uploading)
1. Create a free account at https://github.com and make a new repository.
2. Click "uploading an existing file" and drag in **everything inside** the unzipped folder (not the folder itself). Commit.
3. On https://vercel.com choose "Add New… → Project", pick that repository and press **Deploy**. Leave all settings at their defaults. Framework: "Other". Build command and output directory: empty.

## Using your own domain (optional)
In Vercel: Project → Settings → Domains → add your domain and follow the DNS steps shown.

## What is in the folder
- `index.html`: homepage, skills passage and exhibition room
- `sahaay.html`, `shrunkhala.html`, `boolingo.html`, `fingermask.html`: project pages
- `sahaay/`, `shrunkhala/`, `boolingo/`: images and clips used by those pages
- `Anamika_Shrivastava_Resume.pdf`: the Resume link
- `vercel.json`: hosting settings (already done for you; please do not edit)
- `robots.txt`

## Good to know
- The Finger-Mask experiment asks for camera access. It only works on the live `https://` address (not by double-clicking the file) and loads its hand-tracking library from a public CDN (jsdelivr), so visitors need an internet connection for that page.
- The site loads Google Fonts. Without internet it falls back to system fonts.
- To update the site later, repeat step 5 (Option A) or upload changed files to GitHub (Option B). Vercel republishes automatically.
