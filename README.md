# Saneesh Morais - AI & Software Portfolio

## Overview

A premium, employer-facing portfolio for Saneesh Morais, a First Class Honours Computing with Artificial Intelligence Technology graduate. The site presents nine practical AI, software and data projects as honest product case studies.

## Project purpose

The site helps UK recruiters, hiring managers, founders and technical reviewers understand Saneesh's strongest evidence quickly: practical AI/software/data projects, clear product thinking, and credible junior-level technical range.

## Features

- Dark and light themes with saved preference
- Role-based project recommendations and employer pitch
- Keyword, role and technology filtering
- Nine keyboard-friendly case-study modals
- Reusable project-specific architecture and dashboard previews
- Copyable recruiter pitch and email address
- Responsive layout, scroll reveals and active navigation
- Semantic HTML, accessible controls and reduced-motion support
- SEO, Open Graph and Twitter metadata
- No framework, build step, backend or paid API

## Tech stack

HTML5, CSS3 and vanilla JavaScript. The only external resource is the optional Google Fonts stylesheet; system fonts provide a graceful fallback.

## Project structure

```text
.
|-- index.html
|-- styles.css
|-- script.js
|-- README.md
|-- assets/
|   |-- Saneesh_Morais_CV.pdf
|   `-- favicon.svg
`-- .nojekyll
```

## Run locally

Open `index.html` directly, or serve the folder for the most browser-consistent experience:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy to GitHub Pages

1. Push these files to the root of a GitHub repository.
2. Open **Settings -> Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the relevant branch and `/ (root)`, then save.

No build command is required.

## Update project data

Edit the `projects` array near the top of `script.js`. Each object controls its card and case study.

Role-specific recommendations, pitches, skills and interview prompts are stored in the `roleData` object. Technical strength groups are stored in `skillGroups`.

## Update GitHub and demo links

The project cards currently show honest disabled placeholder buttons for GitHub and demo links. Add verified repository or demo URL fields to the relevant project objects only when they are ready, then update `renderProjects()` to output real anchors for those projects. Do not label a project as a live demo unless the link works.

## Replace project visuals with screenshots

Each generated preview has a `data-replaceable-visual` attribute matching its project ID. To use a verified screenshot later, add the image under `assets/projects/` and update `renderProjectVisual()` in `script.js` for that ID. Keep descriptive `alt` text and retain the surrounding `.project-visual` container so card and modal spacing remains consistent.

## Update the CV PDF

Replace `assets/Saneesh_Morais_CV.pdf` with the latest CV using the same filename. The Download CV button already points to that path.

## Publishing checklist / TODO

- [x] Add the real CV at `assets/Saneesh_Morais_CV.pdf`
- [ ] Add verified GitHub repository URLs per project
- [ ] Add only genuine live demo URLs per project
- [ ] Add project screenshots or short product videos
- [ ] Replace `assets/og-image-placeholder.png` with a 1200 x 630 social image
- [ ] Add the final deployed URL as an `og:url` meta tag
- [ ] Verify all project descriptions against the latest repository state
- [ ] Test the final deployment on mobile and run a Lighthouse audit

## Content principles

The copy deliberately avoids claims of production use, clients, user counts or enterprise deployment. Projects are labelled as prototypes, case studies, code-available work or demo-ready work and should remain that way unless evidence supports a status change.
