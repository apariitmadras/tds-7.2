---
marp: true
title: Product Documentation Presentation
description: Maintainable, version-controlled product docs with Marp
author: Technical Writing Team
theme: product-docs
math: katex
paginate: true
footer: 'Page $page / $pages — Product Docs'
---

<!-- _class: title -->

# ProductName — Developer Guide

**Author:** Technical Writing Team  
**Contact:** 24ds1000011@ds.study.iitm.ac.in

> Version-controlled docs that export cleanly to HTML/PDF/PPTX.

---

<!-- _class: lead -->

## Goals

- Single source of truth in Git  
- Easy conversion to **HTML**, **PDF**, and **PPTX**  
- Consistent look & feel via a **custom theme**  
- Supports **math** (KaTeX) and **code**  
- Production-friendly **page numbers**

---

<!--
_class: spotlight
-->

![bg](assets/hero-cover.jpg)

# Architecture at a Glance

- Modular services
- Clear interfaces
- Observability (logs/metrics/traces)

---

<!-- _class: two-col -->

## Quickstart & Build

**1) Write slides**  
Use this `slides.md` as your base. Commit images to `assets/`.

**2) Export locally**
```bash
# HTML
npx @marp-team/marp-cli slides.md --html --allow-local-files -o dist/slides.html

# PDF (requires Chromium)
npx @marp-team/marp-cli slides.md --pdf --allow-local-files -o dist/slides.pdf

# PPTX
npx @marp-team/marp-cli slides.md --pptx --allow-local-files -o dist/slides.pptx
