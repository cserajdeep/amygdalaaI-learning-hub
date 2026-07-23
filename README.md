# DSA & AI Learning Hub

Interactive learning modules by **Dr. Rajdeep Chatterjee** ([@cserajdeep](https://github.com/cserajdeep)).

## Structure

```
dsa-learning-hub/
├── index.html                     ← Hub landing page (module list)
├── 01-why-dsa/
│   └── index.html                 ← Why DSA matters
├── 02-c-prerequisites/
│   └── index.html                 ← C prerequisites for DSA
└── 03-arrays-in-c/
    └── index.html                 ← Arrays in C + visualizers
```

## Deploying to GitHub Pages

1. Create a new repo under your account, e.g. `dsa-learning-hub`
   (github.com/cserajdeep/dsa-learning-hub).
2. Push this folder's contents to the repo root:
   ```bash
   git init
   git add .
   git commit -m "Initial DSA & AI learning hub"
   git branch -M main
   git remote add origin https://github.com/cserajdeep/dsa-learning-hub.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Source → Deploy from branch → `main` / root**.
4. Your live site will appear at:
   `https://cserajdeep.github.io/dsa-learning-hub/`

Individual module URLs:
- `https://cserajdeep.github.io/dsa-learning-hub/01-why-dsa/`
- `https://cserajdeep.github.io/dsa-learning-hub/02-c-prerequisites/`
- `https://cserajdeep.github.io/dsa-learning-hub/03-arrays-in-c/`

## Adding more modules later

1. Create a new folder, e.g. `04-linked-lists/`, with an `index.html` inside.
2. Add a new card to the `.modules` grid in the root `index.html`.
3. Update the sticky nav bar's "Next"/"Prev" links in `03-arrays-in-c/index.html`
   and the new module page to keep the sequence connected.

## Linking from your Google Site

On `sites.google.com/kiit.ac.in/rajdeep/home`:
- Add a **Button** (or a menu item) labeled "Interactive Learning Hub" pointing to
  `https://cserajdeep.github.io/dsa-learning-hub/` (opens in new tab — recommended), **or**
- Use the **Embed** element → paste the same URL to show it inline on a page.
