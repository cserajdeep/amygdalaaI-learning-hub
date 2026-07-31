# DSA & AI Learning Hub

Interactive learning modules by **Dr. Rajdeep Chatterjee** ([@cserajdeep](https://github.com/cserajdeep)).

## Structure

The hub landing page (`index.html`) now has two top-level tabs — **DSA & C** and **ANN** —
switched entirely client-side (no page reload). Each tab lists its own module cards.

```
dsa-learning-hub/
├── index.html                     ← Hub landing page (DSA & C / ANN tabs)
├── dsa_w_c/
│   ├── 01-why-dsa/
│   │   └── index.html             ← [DSA & C] Why DSA matters
│   ├── 02-c-prerequisites/
│   │   └── index.html             ← [DSA & C] C prerequisites for DSA
│   ├── 03-arrays-in-c/
│   │   └── index.html             ← [DSA & C] Arrays in C + visualizers
│   └── 04-intro-to-ds/
│       └── index.html             ← [DSA & C] Intro to Data Structures
└── ann/
    ├── 01-mcculloch-pitts-neuron/
    │   └── index.html             ← [ANN] McCulloch–Pitts Neuron + logic gates lab
    ├── 02-activation-functions/
    │   └── index.html             ← [ANN] Activation functions + interactive calculator
    ├── 03-perceptron-learning/
    │   └── index.html             ← [ANN] Perceptron learning rule + animated MLP forward pass
    └── 04-adaline-madaline/
        └── index.html             ← [ANN] ADALINE (LMS/delta rule) + MADALINE
```

All module pages share the same dark/light design system, sticky section nav-bar, and
card/badge/formula components (see `dsa_w_c/03-arrays-in-c/index.html` for the canonical template).

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
- `https://cserajdeep.github.io/dsa-learning-hub/dsa_w_c/01-why-dsa/`
- `https://cserajdeep.github.io/dsa-learning-hub/dsa_w_c/02-c-prerequisites/`
- `https://cserajdeep.github.io/dsa-learning-hub/dsa_w_c/03-arrays-in-c/`
- `https://cserajdeep.github.io/dsa-learning-hub/dsa_w_c/04-intro-to-ds/`
- `https://cserajdeep.github.io/dsa-learning-hub/ann/01-mcculloch-pitts-neuron/`
- `https://cserajdeep.github.io/dsa-learning-hub/ann/02-activation-functions/`
- `https://cserajdeep.github.io/dsa-learning-hub/ann/03-perceptron-learning/`
- `https://cserajdeep.github.io/dsa-learning-hub/ann/04-adaline-madaline/`

## Adding more modules later

**DSA & C track:**
1. Create a new folder under `dsa_w_c/`, e.g. `dsa_w_c/05-linked-lists/`, with an `index.html` inside.
2. Add a new card to the `#panel-dsa .modules` grid in the root `index.html`, linking to
   `dsa_w_c/05-linked-lists/index.html`.
3. Update the sticky nav bar's "Next"/"Prev" links in the last DSA module page
   and the new module page to keep the sequence connected (note: "Hub Home" from inside
   `dsa_w_c/*/` uses `../../index.html`, while sibling module links use `../`).

**ANN track:**
1. Create a new folder under `ann/`, e.g. `ann/05-hopfield-networks/`, with an `index.html` inside.
2. Add a new card to the `#panel-ann .modules` grid in the root `index.html`.
3. Update the sticky nav bar's "Next"/"Prev" links in `ann/04-adaline-madaline/index.html`
   and the new module page (note the `../../index.html` relative path back to hub home
   from inside `ann/*/`).

## Linking from your Google Site

On `sites.google.com/kiit.ac.in/rajdeep/home`:
- Add a **Button** (or a menu item) labeled "Interactive Learning Hub" pointing to
  `https://cserajdeep.github.io/dsa-learning-hub/` (opens in new tab — recommended), **or**
- Use the **Embed** element → paste the same URL to show it inline on a page.
