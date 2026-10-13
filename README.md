# reymedillo.github.io

Personal profile and portfolio site for **Rey Mark Medillo**, Full Stack Developer based in Perth, Western Australia.

**Live site:** https://reymedillo.github.io/

## About

A single-page static site covering:

- **Experience** – career timeline, from Evaran (previously Health Metrics) back to 2010
- **Projects** – selected client and personal projects (Laravel, Golang, MEAN, EC-CUBE and more)
- **Skills** – programming languages, databases, cloud (AWS Certified Solutions Architect – Associate) and tooling
- **Education**
- **Get in touch** – contact details and a contact form

Built on the [Hyperspace](https://html5up.net/hyperspace) template by HTML5 UP. Plain HTML, CSS and jQuery, with no build step.

## Project structure

```
.
├── index.html              # The whole site
├── assets/
│   ├── css/
│   │   ├── main.css        # Hyperspace template styles (unmodified)
│   │   └── custom.css      # Site-specific styles: profile photo, timeline, tags, project cards
│   ├── js/                 # Template scripts (jQuery, scrolling, breakpoints)
│   ├── sass/               # Template SCSS sources (reference only, not compiled)
│   └── webfonts/           # Font Awesome
├── images/
│   └── profile.png         # Profile photo
├── favicon.ico             # Favicon (16/32/48px)
├── favicon-32x32.png
├── apple-touch-icon.png    # iOS home screen icon
├── .nojekyll               # Tells GitHub Pages to serve files as-is
└── LICENSE.txt             # Template license (CCA 3.0)
```

## Running locally

Open `index.html` in a browser, or serve the folder to mirror GitHub Pages:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

## Updating content

All content lives in `index.html`, split into commented sections (`<!-- Experience -->`, `<!-- Projects -->`, etc.):

- **New job:** add an `<li>` at the top of the `timeline` list in the Experience section.
- **New project:** add a `<section>` inside `<div class="features projects">`. Icons use [Font Awesome 5 Free](https://fontawesome.com/v5/search?m=free) class names, e.g. `fa-code`.
- **Styling tweaks:** put them in `assets/css/custom.css` and leave `main.css` untouched, so template updates stay easy.

## Contact form

The form in the **Get in touch** section isn't connected yet, because GitHub Pages can't process form submissions. To enable it:

1. Create a free form endpoint with a service such as [Formspree](https://formspree.io/).
2. In `index.html`, replace `action="#"` on the contact form (marked with a `TODO` comment) with the endpoint URL.

## Deployment

The site deploys automatically with GitHub Pages from the `main` branch (root folder). Push to `main` and the live site updates within a minute or two.

```bash
git add .
git commit -m "Update site content"
git push
```

## Credits

- Template: [Hyperspace](https://html5up.net/hyperspace) by [HTML5 UP](https://html5up.net), free under the [Creative Commons Attribution 3.0 License](https://html5up.net/license). The footer credit must stay in place.
- Icons: [Font Awesome](https://fontawesome.com) Free.
