# Marcus Toh’s Portfolio

A Jekyll portfolio using the Minimal Mistakes remote theme, hosted on GitHub Pages.

## Local Preview

Use Ruby 3.3 and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve --livereload
```

Open http://localhost:4000/. Restart the server after editing `_config.yml`.

## Editing Content

- Homepage: `_pages/about.md`
- Resume: `_pages/resume.md`
- Projects index: `_pages/projects.md`
- Project articles: `_projects/*.md`
- Project article layout: `_layouts/project.html`
- Navigation: `_data/navigation.yml`
- Site settings and social links: `_config.yml`
- Images: `assets/images/`

To add a project, copy an existing file in `_projects/`, give it a unique filename,
and edit its title, excerpt, context, order, technologies, and content. The filename
sets its URL, such as `/projects/snackapp/`. It appears in the project index automatically.
Replace `project_image` and `project_image_alt` to use your own project image.

The homepage is served at `/`; the old `/about/` address redirects there.

## Before Publishing

```sh
JEKYLL_ENV=production bundle exec jekyll build
```

Commit the source files, including new project articles, layouts, and images.
Do not edit or upload `_site/`; Jekyll generates it. The remote theme needs network
access during builds. Project illustrations currently include intentional placeholders.
