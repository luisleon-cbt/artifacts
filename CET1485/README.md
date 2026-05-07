# CET1485 — Network Essentials

**Course materials repository for CET1485 Network Essentials at CBT Technology Institute · School of Technology**

This repository hosts the interactive learning artifacts for the course. Each module/week has its own folder containing browser-based interactive simulators that students access through Canvas LMS.

---

## About this course

CET1485 Network Essentials introduces students to the foundational concepts of computer networking: how data moves between devices, the equipment that makes networks work, and the practical skills needed to set up and maintain a small network. The course builds the technical and conceptual base required for advanced coursework — including CET1588 Network+ Cert Prep — and prepares students for entry-level roles in IT support and network technician work.

| Field | Value |
|---|---|
| Course code | CET1485 |
| Course name | Network Essentials |
| Program | Networking Administration · Computer Network Support Specialist |
| School | School of Technology |
| Institution | CBT Technology Institute |
| Delivery | Blended (50% online, 50% on-campus) |

---

## Repository structure

Artifacts are organized by week and session. Each session folder holds the interactive HTML files that are embedded into Canvas pages via iframe.

```
cet1485-network-essentials/
├── README.md
├── week-01/
│   ├── session-01-online/
│   │   └── [interactive artifacts...]
│   └── session-02-campus/
│       └── [interactive artifacts...]
├── week-02/
│   ├── session-03-online/
│   └── session-04-campus/
└── ...
```

Sessions follow the course schedule: half are delivered online (asynchronous, self-paced) and half on-campus (instructor-led, lab-intensive).

---

## How these artifacts are used

The artifacts in this repository are **not standalone learning materials**. They are designed to be embedded into Canvas LMS pages via iframe. The Canvas page provides the context, learning objectives, and surrounding instructions; the iframe delivers the interactive experience.

### Hosting

This repository is published via **GitHub Pages**. Once Pages is enabled, files are publicly accessible at:

```
https://[your-github-username].github.io/cet1485-network-essentials/week-XX/session-XX-mode/[filename].html
```

That URL gets dropped into the `src` attribute of the iframe in the matching Canvas page.

### Iframe markup used in Canvas pages

```html
<p title="embedded content">
  <iframe style="border: 1px solid #ccc; min-height: 1500px;"
          src="[full URL to the artifact]"
          width="100%" height="1500"
          loading="lazy"
          allowfullscreen="allowfullscreen"
          data-mce-fragment="1">
  </iframe>
</p>
```

---

## Technical notes

- All artifacts are **single-file HTML** — HTML, inline CSS, and inline JavaScript in one file. No build step, no dependencies, no server required.
- **Light theme** by default with CBT Technology Institute brand styling.
- Designed to meet **WCAG 2.1 AA** accessibility standards: keyboard navigation, screen-reader compatibility, color contrast above minimums, captions/alt text where applicable.
- Compatible with modern browsers (Chrome, Firefox, Edge, Safari).
- Mobile-responsive within the iframe constraint.

---

## Updates and caching

Changes to artifacts are committed and pushed to this repository. **GitHub Pages caches aggressively**, so updates may take a few minutes to propagate after a push. During testing, force-refresh with `Ctrl+Shift+R` (Windows/Linux) or `Cmd+Shift+R` (macOS) to bypass the cache.

---

## Use and attribution

These materials are developed for use at CBT Technology Institute. Faculty and students of CBT have full access to use these artifacts as part of their coursework. Direct linking to artifacts hosted here is permitted from official CBT Canvas courses.

---

*Developed by Professor De León · [professordeleon.blog](https://professordeleon.blog) · Course materials for CBT Technology Institute · School of Technology · © 2026*
