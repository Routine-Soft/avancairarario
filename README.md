# Avançai Rara Rio — Website

Website of **Avançai**, the discipleship track of **Igreja Comunhão Rara Rio**. Members watch the lessons of each module (Start, Reset and CDV), answer the questionnaires and download the study booklets.

![HTML](https://img.shields.io/badge/html-5-E34F26?logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/css-3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-vanilla-F7DF1E?logo=javascript&logoColor=black)
![Vercel](https://img.shields.io/badge/deploy-vercel-000000?logo=vercel)

## Demo

- **Website:** https://avancairarario.vercel.app/

![Avançai website](https://github.com/user-attachments/assets/0f6a9201-a32b-4cd5-8a29-075007b4a42f)
![Avançai website 2](https://github.com/user-attachments/assets/cdc44a1b-6878-4ebf-9c4d-9d3ed2f09c8c)

## Features

- **Home page** presenting the Avançai track.
- **Three modules:** Start, Reset and CDV, each with its own page.
- **Video lessons** (YouTube) shown one at a time.
- **Questionnaires** for each lesson.
- **Study booklets** in PDF to download (`apostilas/`).
- **Top navigation menu** shared by all pages.
- **Responsive layout** for phones.

## Tech stack

| Area | Technology |
|---|---|
| Pages | Plain HTML |
| Styles | Plain CSS (plus `responsive.css` for phones) |
| Scripts | Vanilla JavaScript (one file per module) |
| Videos | YouTube embeds |
| Hosting | Vercel |

No framework, no bundler and no `package.json`.

## Prerequisites

- A modern browser
- Optional: any static file server to test locally (for example `npx serve`)

## Installation

```bash
git clone <repository-url> avancairarario
cd avancairarario
npx serve .
```

Then open the address shown in the terminal. Shared parts (menu, header) are loaded with JavaScript, so use a local server instead of opening the files directly.

## Configuration

There are no environment variables. The website is public and must never contain secrets.

## Usage

- Edit the HTML/CSS/JS files and refresh the browser: there is no build.
- **Lessons:** each module's lessons (title, video and questionnaire button) are defined in `js/start.js`, `js/reset.js` and `js/cdv.js`.
- **Booklets:** replace the PDFs in `apostilas/` keeping the same file names.

## Folder structure

```
avancairarario/
├── index.html            # Home page
├── views/                # Module pages (start, reset, cdv) and the top menu
├── components/           # Shared header
├── js/                   # Lessons of each module
├── css/                  # Home, modules, questionnaires, tests, menu and responsive styles
├── apostilas/            # Study booklets (PDF)
└── img/                  # Logo and images
```

## Deployment

- Hosted on **Vercel**. Every push to `main` publishes automatically, with no build step.

## Contributing

1. Create a branch from `main`: `feature/<name>` (or `fix/<name>`).
2. Keep one script per module in `js/` and one page per module in `views/`.
3. Test on a phone-sized screen.
4. Write commit messages in Portuguese and open a pull request to `main`.

## License and author

**Private and proprietary.** All rights reserved. Content, videos and booklets belong to Igreja Comunhão Rara Rio.

Developed by **Stanley Andrade**.
