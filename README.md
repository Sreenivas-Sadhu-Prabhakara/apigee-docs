# Apigee Docs — public engineering docs

This repository hosts the **public documentation** for an Apigee X FAPI 1.0 Advanced chassis, a
private Apigee X reference chassis that implements **FAPI 1.0 Advanced** for UK Open
Banking. The pages here explain the architecture, the FAPI security model, every
shared flow, the reference proxy, deployment/testing, and the CI/CD + IAM model — so
the design can be read, reviewed, and learned from without exposing the implementation.

## What is published here vs. what stays private

- **Published (this repo):** narrative engineering docs as static HTML — architecture,
  security model, per-shared-flow guides (`sf-*`), the reference proxy walkthrough,
  deployment & testing, CI/CD & IAM, and build decisions.
- **Private by design (not in this repo):** the chassis itself (private code repository) —
  proxy bundles, shared-flow XML, policy configuration, pipelines, and any
  environment/credential material. The code is intentionally kept private; these docs
  describe it but do not ship it.

## How it's served

Served as a static site via **GitHub Pages** straight from the repository root. The
`.nojekyll` marker disables Jekyll processing so files under `assets/` are served
verbatim. `index.html` is the entry point; every page shares the same sidebar nav and
the `assets/styles.css` stylesheet.

## Build

No build step — author/edit the static HTML directly and push; GitHub Pages serves the
files as-is.
