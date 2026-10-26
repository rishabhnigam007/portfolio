# Project Plan

## Goal

Build and publish a polished, easy-to-maintain personal portfolio for Rishabh Nigam. The initial static site is implemented; publish it on GitHub Pages, then connect a custom domain when one is available.

## Scope

The portfolio is a fast, accessible static website drafted from the owner's signed-in LinkedIn profile. The owner should review the content and metrics before publication. The layout is designed to make professional experience and selected work easy to scan on desktop and mobile.

### Planned sections

- Home: name, professional headline, and primary links
- About: concise professional introduction
- Experience: roles, organizations, dates, and impact
- Projects: selected work, contribution, technologies, and links
- Skills: grouped, relevant skills
- Education and certifications: include only items the owner wants displayed
- Contact: email and professional/social links approved for publication

Final section names and order can change to fit the available profile content.

## Technology and maintainability

- Use semantic HTML and plain CSS for structure and site-specific styles.
- Use Tailwind CSS and Bootstrap as requested, with an explicit division of responsibilities.
- Avoid duplicate framework resets: configure Tailwind Preflight appropriately if Bootstrap's Reboot is used.
- Keep content and repeated presentation patterns straightforward to edit.
- Use responsive layouts, keyboard-accessible navigation, descriptive links, and adequate color contrast.
- Choose a purposeful font pairing with strong readability, clear heading hierarchy, and sensible line lengths. Confirm font licensing and provide fallbacks.
- Optimize images and avoid adding a backend or paid hosting dependency.

## Phases

1. **Review content**: confirm details and quantified outcomes in [CONTENT.md](CONTENT.md), and choose a durable local profile photo.
2. **Review the design**: check typography, colors, and responsive layouts on mobile and desktop.
3. **Build**: run `npm install` and `npm run build` to generate `tailwind.css`.
4. **Publish on GitHub Pages**: create or use a GitHub repository, push the static site, enable Pages, and verify the public URL.
5. **Add a custom domain later**: configure the domain in GitHub Pages and set DNS at the registrar; verify HTTPS.

## Completion checklist

- [x] Profile details collected and the first static site built.
- [ ] Owner has approved all personal and professional details for publication.
- [ ] All external links and contact methods are confirmed.
- [x] Responsive layout and typography are reviewed on mobile and desktop.
- [x] No placeholder copy or broken internal links remain.
- [ ] GitHub Pages URL works over HTTPS.
- [ ] Optional custom domain resolves and HTTPS works when configured.
