# My-portofolio
A personal portfolio website for Osman Adam, a junior web developer based in Pau, France. It showcases his professional profile, skills, and three main projects (Orthalist, a dashboard template, and a WhatsApp contact form) with case study pages for each.

### Stack
- **Language(s):** HTML (56%), CSS (22%), SCSS (21%), JavaScript (1.6%)
- **Framework / runtime:** Static HTML site with vanilla JavaScript
- **Notable features:** SCSS-based styling with modular architecture, responsive design, hamburger menu for mobile, client-side form validation

## How it's organized

```
index.html                    Main landing page with hero, about, projects, contact sections
index.js                      Hamburger menu toggle and navigation logic
project-*.html               Case study pages for Orthalist, dashboard, and form projects
css/
  style.css                   Compiled stylesheet from SASS
sass/
  main.scss                   Entry point importing subdirectories
  abstracts/                  Variables, mixins, functions
  base/                       Reset, typography, base element styles
  components/                 Reusable component styles
  pages/                      Page-specific styles
assets/
  jpeg/                       Project screenshots and profile images
  png/                        Social media icons
  svg/                        Hamburger menu icons
```

**How it fits together:** The site is a traditional multi-page static website. `index.html` is the main entry point with sections for hero, about, projects, and contact. Navigation is handled by `index.js`, which toggles a mobile hamburger menu. Each project has its own HTML page linked from the projects section. Styling is compiled from SCSS using a 7-1 architecture pattern (abstracts, base, components, pages).

## How to run it
Since this is a static site, just open `index.html` in a browser:

```bash
# Clone and open locally
git clone https://github.com/osmanadam-dev/My-portofolio
cd My-portofolio
open index.html
# or just open it in your browser directly

# For SCSS development, compile with:
sass sass/main.scss css/style.css --watch
```

No build process, server, or dependencies required—the site runs directly in the browser.
