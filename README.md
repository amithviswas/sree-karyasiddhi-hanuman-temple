# Sree Karyasiddhi Hanuman Temple: Community Website

A bilingual (English / Telugu) website for the **Sree Karyasiddhi Hanuman Temple**, a community temple under construction in Radhayapalem, Rajanagaram Mandal, East Godavari, Andhra Pradesh, run by the Sree Karyasiddhi Hanuman Trust. The site tells the temple's story, follows its construction progress, introduces the people behind it, and makes it easy for devotees to donate.

**Live site:** https://amithviswas.github.io/sree-karyasiddhi-hanuman-temple/

## Features
- **English / Telugu toggle**: a language picker on first visit, a switch in the header, and the choice remembered in `localStorage`.
- **Sections**: About the Temple, About Lord Hanuman, The People Behind It, a Construction Journey timeline (Bhoomi Puja → foundation → idol construction → current stage), Photo Gallery, and "Be a Part of This Temple".
- **Photo gallery lightbox** with keyboard and swipe (touch) navigation.
- **Donations**: UPI deep links (including preset amounts) that open the visitor's UPI app on mobile, bank-transfer details, and one-tap copy-to-clipboard.
- Tap-to-call contact links, a scroll hint and small decorative animations (petal shower).
- Responsive, mobile-first layout; Open Graph tags for rich link previews on WhatsApp and social media.
- Single self-contained `index.html` (inline CSS and JavaScript), so there's no build step.

## Tech stack
- HTML5, CSS3, vanilla JavaScript
- WebP / JPEG images
- Hosted on GitHub Pages

## Run locally
```bash
git clone https://github.com/amithviswas/sree-karyasiddhi-hanuman-temple.git
cd sree-karyasiddhi-hanuman-temple
# open index.html in a browser, or serve it:
python -m http.server 8000
```

## Project structure
```
.
├── index.html            # the whole site: markup, styles and scripts
├── favicon.svg
├── images/               # temple, idol and ceremony photos (WebP) + og-image.jpg
├── Construction/         # construction progress photos
└── people behind it/     # photos of the founder / trustees
```

## Updating content
- Construction milestones, gallery items and donation details are edited directly in `index.html`. Each text block has an English (`.en`) and a Telugu (`.te`) version.
- Add new photos to `images/` or `Construction/` and reference them from the gallery / timeline markup.
- Pushing to the default branch updates the GitHub Pages site.

## Author
Website designed and built by **Amith Viswas Reddy**, Salesforce engineer at Accenture.
- Portfolio: [avr-portfolio-m5.netlify.app](https://avr-portfolio-m5.netlify.app)
- LinkedIn: [linkedin.com/in/amith-viswas-reddy](https://www.linkedin.com/in/amith-viswas-reddy)
- GitHub: [@amithviswas](https://github.com/amithviswas)

## License
Website code is released under the [MIT License](LICENSE). Temple photographs and content belong to the Sree Karyasiddhi Hanuman Trust.
