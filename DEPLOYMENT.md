# Deployment Guide

## GitHub Pages: initial free hosting

GitHub Pages can host a static portfolio at no hosting cost for a public repository. The eventual GitHub account or repository URL is not known yet, so update the examples below once the repository is created.

1. Create a GitHub repository for the portfolio. A repository named `username.github.io` can use the account's root Pages URL; another repository is typically published under `https://username.github.io/repository-name/`.
2. Run `npm install` and `npm run build` locally to generate `tailwind.css` from `tailwind.input.css`.
3. Add the completed static site, including the generated `tailwind.css`, and push the default branch to GitHub.
4. In the repository, open **Settings → Pages**.
5. Choose **Deploy from a branch**, then select the branch and folder containing `index.html`.
6. Wait for deployment and open the Pages URL shown in the settings. Check that the home page, image, stylesheets, and internal links load correctly.
7. Keep relative asset paths compatible with a repository subpath if using a project Pages URL.

GitHub Pages is static hosting. This project does not require a server or database. Check GitHub's current Pages limits and terms before publishing.

## Custom domain: later step

A custom domain is optional and requires purchasing/renewing a domain through a registrar; GitHub Pages hosting itself remains free.

1. Choose the domain and decide whether the root domain, `www`, or both should work.
2. In **Settings → Pages**, enter the custom domain and save it. GitHub may create or update a `CNAME` file in the published source.
3. At the domain registrar, add the DNS records recommended by GitHub for the chosen domain type. For a root/apex domain, this commonly involves GitHub Pages A/AAAA records; for a subdomain such as `www`, it commonly uses a CNAME pointing to the GitHub Pages hostname. Use GitHub's current documentation for exact values.
4. Wait for DNS propagation, then verify the domain in GitHub Pages settings.
5. Enable **Enforce HTTPS** when the option becomes available and test both the custom domain and the GitHub Pages URL.
6. If using both root and `www` domains, configure the preferred canonical domain and confirm the other redirects as expected.

Do not publish registrar credentials or other secrets in this repository. DNS changes can take time to propagate.
