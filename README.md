# Become an Agentic Architect – Course Page

This repository hosts the public **Course Page** and **Wall of Fame** for capstone projects built in Carmelo Iaria’s Maven course
[“Become an Agentic Architect”][course].

The site is published via GitHub Pages at:

> https://synaptic-ai-consulting.github.io/become-an-agentic-architect-projects/

[course]: https://maven.com/carmelo-iaria/agentic-architect

---

## What this repo contains

- `index.html`  
  The Course Page: alumni world map, HTML review wall, published capstones, instructor, syllabus. Lime flags with an eye icon open a published capstone in a modal. Map zoom is click-to-enable so page scroll is not trapped.

- `wall-of-fame.html`  
  The original card gallery. It reads from `projects.json` to render cards client-side.

- `syllabus.json`  
  Week-by-week syllabus captured from the live Maven listing.

- `assets/`  
  Map data, review manifest, instructor portrait/badge, Maven logo. Regenerated from the private marketing repo with `npm run wall-of-fame-publish` (operator only).

- `projects.json`  
  One entry per published project (title, author, cohort, hero image, showcase URL).

- `projects/<slug>/`  
  One folder per project, where `<slug>` is a URL-friendly identifier, for example:

  ```text
  projects/jan26-onboarding-crew-jane-doe/
    index.html      # project showcase page
    hero.png        # main thumbnail shown on the gallery card
    screen-1.png
    screen-2.png
    ...
  ```

---

## Contributing

Students must:

1. **Use the provided Cursor prompt** when building the capstone.
2. **Add a unique `projects/<slug>/` folder** (e.g. `projects/jan26-onboarding-crew-jane-doe/`) with the showcase page and assets.
3. **Append a valid JSON object to `projects.json`** so the project appears on the Wall of Fame.
4. **Commit & push to `main`** to submit the project.
