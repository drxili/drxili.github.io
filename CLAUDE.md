# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Xi Li's personal homepage, deployed as a GitHub Pages **user site** at `https://xili.github.io`. Because the repo is named `<username>.github.io`, GitHub serves the site from the default branch root — no `docs/` folder or project-page path prefix.

## Status

Repository is empty. No stack has been chosen yet. Before scaffolding, confirm with the user which approach they want:

- **Plain static HTML/CSS/JS** — simplest, no build step, GitHub Pages serves files as-is.
- **Jekyll** — GitHub Pages' built-in default; auto-builds on push, no Actions workflow needed. Use if the user wants Markdown posts/pages with minimal tooling.
- **Other static-site generator** (Astro, Hugo, Eleventy, Next.js static export, etc.) — requires a GitHub Actions workflow to build and publish to the `gh-pages` branch or via the Pages deployment action.

The choice determines the build commands, directory layout, and CI setup — do not assume one.

## Deployment

GitHub Pages publishes automatically from the configured branch (Settings → Pages on github.com). For non-Jekyll stacks, a workflow under `.github/workflows/` is required. If you add one, prefer the official `actions/deploy-pages` flow over pushing to `gh-pages` manually.

If the site uses Jekyll and you want to skip Jekyll processing for a file or directory (e.g., to serve a raw `_folder`), add an empty `.nojekyll` file at the repo rootTo 

## To do

1. 2026-05-05: Create a github page for Xi Li
   1. Use the style of daojing zhai https://daojingzhai.github.io/
   2. Xi Li is a PhD student in princeton: https://scholar.google.com/citations?user=d0t8yiAAAAAJ&hl=en
   3. Avatar use the photo of Xi Li in Rabinowitz's website. https://chemistry.princeton.edu/faculty-research/faculty/joshua-rabinowitz/.
   4. For each paper, use hyperlink to the publication. Give abstract like Daojing.
   5. Finally create a page on Github, my Github account: Xili-hope
