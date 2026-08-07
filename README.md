# Portfolio template

A single-file, dependency-free portfolio site (`index.html`) styled like an
engineer's notebook — graph-paper background, route-style section labels,
and a git-log-styled experience timeline. Sample content is for a fictional
backend engineer, "Maya Chen" — replace it with your own.

## Customize

Open `index.html` and edit directly — everything lives in one file:

- **Name, role, tagline** — top of the `<body>`, in the `.hero` section.
- **About + meta panel** — `#about` section.
- **Projects** — `#work` section, one `<article class="project">` per project.
- **Experience** — `#experience` section, one `.commit` block per role.
- **Skills** — `#skills` section, grouped lists.
- **Contact** — `#contact` section: swap the email, GitHub, LinkedIn, and resume links.
- **Colors** — all defined as CSS variables at the top of the `<style>` block
  (`--paper`, `--ink`, `--stamp`, `--teal`, etc.) if you want a different palette.

If you have a resume PDF, drop it in this folder as `resume.pdf` — it's already linked.

## Deploy to GitHub Pages

1. Create a new repository on GitHub. For a personal site at
   `https://<username>.github.io`, name the repo exactly `<username>.github.io`.
   For a project page instead, any repo name works — it'll be served at
   `https://<username>.github.io/<repo-name>/`.
2. Push these files to the repo's default branch (usually `main`):
   ```bash
   git init
   git add index.html README.md
   git commit -m "Add portfolio site"
   git branch -M main
   git remote add origin https://github.com/<username>/<repo-name>.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to "Deploy from a branch",
   pick `main` and `/ (root)`, then save.
5. GitHub will publish the site within a minute or two at the URL shown on
   that same Pages settings screen.

No build step is required — it's plain HTML/CSS/JS.
