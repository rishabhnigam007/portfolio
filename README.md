# Rishabh Nigam | Portfolio

A responsive personal portfolio website for presenting Rishabh Nigam's backend engineering experience, projects, skills, and public LinkedIn link. The static site is designed for GitHub Pages hosting.

## Project status

First portfolio version implemented from the profile sections visible in the owner's signed-in LinkedIn session. See [CONTENT.md](CONTENT.md) for the source summary and items that still need owner review.

## Planned technology

- HTML for semantic page structure
- CSS for site-specific styling
- Tailwind CSS compiled locally with its preflight reset disabled
- Bootstrap 5 grid and responsive layout utilities via CDN

Tailwind and Bootstrap will be configured to avoid competing resets and styles. Keep component ownership clear and use a small, consistent set of patterns rather than mixing both frameworks on the same elements without a reason.

## Documentation

- [Project plan](PROJECT_PLAN.md): scope, structure, and implementation steps
- [Content inventory](CONTENT.md): profile content and assets to gather
- [Deployment guide](DEPLOYMENT.md): GitHub Pages setup and later custom-domain configuration
- [Step-by-step deployment instructions](DEPLOYMENT.txt): PowerShell, GitHub Pages, registrar DNS, and HTTPS setup

## Getting started

Install the development dependency and generate the Tailwind stylesheet before publishing:

```sh
npm install
npm run build
```

Open `index.html` locally or follow [DEPLOYMENT.md](DEPLOYMENT.md) to publish the static site. Review dates, achievement metrics, the profile photo, and the selected public content before deployment.
