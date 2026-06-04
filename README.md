# Hello, I'm James 👋 

I’m a design leader who helps organisations build great in-house teams and digital services. 20+ years’ experience delivering software systems, defining design practices, and developing people.

[hellojames.co.uk](https://hellojames.co.uk)

---

## Stack

- **Generator:** Jekyll
- **Hosting:** GitHub Pages
- **Domain:** Custom CNAME → `hellojames.co.uk`
- **Languages:** HTML, CSS
- **Fonts:** Georgia, [Anonymous Pro](https://fonts.google.com/specimen/Anonymous+Pro) via Google Fonts
- **Plugins:** `jekyll-redirect-from`

## Structure

```
├── _config.yml        # Jekyll site configuration
├── _includes/         # Reusable HTML partials
├── _layouts/          # Page layout templates
├── colophon/          # Colophon
├── media/             # Static assets & downloadable files
├── writing/           # Writings
├── index.html         # Homepage
├── CNAME              # GitHub Pages custom domain config
└── .gitignore
```

## Running locally

Requires Ruby and Bundler.
```
bash
bundle install
bundle exec jekyll serve
```

Available at `http://localhost:4000`.

## Deployment

Pushing to `main` deploys automatically via GitHub Pages. No CI pipeline required.

