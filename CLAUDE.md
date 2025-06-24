# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MENTOR.page is a research paper project website for "MENTOR: Efficient Multimodal-Conditioned Tuning for Autoregressive Vision Generation Models". The repository contains:
- A static website (`index.html`) hosted on GitHub Pages
- LaTeX paper submission files for NeurIPS in `/NeurIPS-VidualInstructionEditing/`
- Static assets (CSS, JavaScript, images) in `/static/` and `/bower_components/`

## Common Development Tasks

### Website Development
- **Edit Website**: The main website file is `index.html` at the root
- **CSS Styles**: Custom styles are in `/static/css/index.css`
- **JavaScript**: Interactive features are in `/static/js/index.js`
- **Images**: Store website images in `/static/images/`

### LaTeX Paper Compilation
- **Main File**: `/NeurIPS-VidualInstructionEditing/main.tex`
- **Build Command**: `pdflatex main.tex` (run from the LaTeX directory)
- **Bibliography**: `bibtex main` after initial compilation
- **Sections**: Paper sections are in `/NeurIPS-VidualInstructionEditing/sections/`
- **Figures**: Paper figures are in `/NeurIPS-VidualInstructionEditing/figures/`

## Code Architecture

### Website Structure
- Single-page website using Bulma CSS framework
- Sections: Hero, News, Overview, Highlights, Why MENTOR, Method, Results, Efficiency, Comparison, Citation
- Uses FontAwesome for icons and Google Fonts for typography
- No build process required - pure HTML/CSS/JS

### LaTeX Paper Structure
- Uses NeurIPS 2024 template (`neurips_2024.sty`)
- Modular section files in `/sections/` directory
- Custom commands defined: `\model` for MENTOR, `\cmark` for checkmarks
- Author comments system: `\haozhe{}`, `\zefan{}`, `\junjie{}`

## Key Files and Locations
- `index.html`: Main website file
- `/NeurIPS-VidualInstructionEditing/main.tex`: LaTeX paper main file
- `/NeurIPS-VidualInstructionEditing/ref.bib`: Bibliography
- `/static/css/index.css`: Custom website styles
- `/static/images/`: Website images (method.png, main_results.png, comparison.png)
- `/NeurIPS-VidualInstructionEditing/figures/`: Paper figures

## GitHub Pages Deployment
The website is served directly from the repository root. Any changes to `index.html` or static assets will be reflected on the live site after pushing to the main branch.