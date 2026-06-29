# Apigee Docs

Documentation hub for **Apigee X** — reference documentation for building
production-grade APIs on Apigee X. Served as a static site via GitHub Pages.

## Structure

```
apigee-docs/
├── index.html        # hub landing — lists the documentation sets
├── assets/
│   └── styles.css    # shared design system (used by every page)
└── chassis/          # doc set: FAPI 1.0 Advanced shared-flow security chassis
    ├── index.html        # overview & request lifecycle
    ├── architecture.html
    ├── security-model.html
    ├── sf-*.html         # one page per shared flow
    ├── reference-proxy.html
    ├── deployment.html
    ├── cicd-iam.html
    └── decisions.html
```

## Adding a new documentation set

1. Create a folder at the repo root (e.g. `mytopic/`).
2. Reference the shared stylesheet from each page with `../assets/styles.css`.
3. Add a card linking to it in the root `index.html`.

## Scope

This repository is for Apigee X **documentation** only. Hands-on **training
courses are maintained in their own separate repositories** and are not part of
this site.

> Examples in these docs use generic placeholders (`your-org`,
> `your-apigee-project`, `your-eval-host`, `auth.example.com`). Substitute your
> own values when applying them.

## How it's served

Static site via **GitHub Pages** from the repository root. The `.nojekyll` marker
disables Jekyll so files under `assets/` are served verbatim. No build step —
edit the HTML and push.
