# anitasoaares.github.io

Personal portfolio website of **Ana Soares Dias**, Full Stack Software Engineer based in Braga, Portugal.

Live site: <https://anitasoaares.github.io>

## Overview

A static, responsive single-page portfolio built with plain HTML, CSS and JavaScript, hosted on GitHub Pages. It presents an about section, skills, resume, certifications, services and a contact form.

## Pages

| File | Description |
| --- | --- |
| `index.html` | Main page with the Hero, About, Skills, Resume, Certifications, Services and Contact sections |
| `certifications.html` | Full, filterable list of courses and certifications with certificate previews |
| `portfolio-details.html` | Detail page for an individual portfolio item |
| `service-details.html` | Detail page for an individual service |

## Project structure

``` bash
.
├── index.html
├── certifications.html
├── portfolio-details.html
├── service-details.html
├── assets/
│   ├── css/main.css        # Site styles
│   ├── img/                # Images (profile, portfolio, certifications)
│   ├── js/main.js          # Navigation, scroll effects, filters, form handling
│   └── vendor/             # Third-party libraries (see below)
└── forms/
    └── contact.php         # Server-side handler for the contact form
```

## Built with

- [Bootstrap 5](https://getbootstrap.com/) and [Bootstrap Icons](https://icons.getbootstrap.com/)
- [AOS](https://michalsnik.github.io/aos/) – scroll animations
- [GLightbox](https://biati-digital.github.io/glightbox/) – lightbox for certificates and images
- [Isotope](https://isotope.metafizzy.co/) + [imagesLoaded](https://imagesloaded.desandro.com/) – filterable layouts
- [Swiper](https://swiperjs.com/) – sliders
- [Typed.js](https://mattboldt.com/demos/typed-js/) – animated hero text
- [PureCounter](https://github.com/srexi/purecounterjs) – animated counters
- [Waypoints](http://imakewebthings.com/waypoints/) – scroll triggers

All vendor libraries are committed under `assets/vendor/`, so there is no build step or package manager.

## Running locally

No dependencies or build tooling are required. Clone the repository and serve the folder with any static server:

```bash
git clone https://github.com/anitasoaares/anitasoaares.github.io.git
cd anitasoaares.github.io

# Python
python -m http.server 8000
```

Then open <http://localhost:8000>.

Opening `index.html` directly in a browser also works, though a local server is recommended so relative paths and scripts behave exactly as they do in production.

## Contact form

The contact form posts to `forms/contact.php`, which requires a PHP-enabled host and the `PHP Email Form` library. GitHub Pages serves static files only, so the form will not send email from the GitHub Pages deployment — replace it with a hosted form service (for example Formspree or Netlify Forms) or deploy to a PHP-capable host if email delivery is needed.

## Deployment

The site is published automatically by GitHub Pages from the default branch. Pushing to that branch updates the live site.

## License

Content, images and text are © Ana Soares Dias. Third-party libraries under `assets/vendor/` retain their own licenses.
