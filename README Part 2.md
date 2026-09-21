# PixelCart Digital Solutions - Website Project

## Project Title
PixelCart Digital Solutions Website (WEDE5020 Portfolio of Evidence)

## Student Information
- Full Name: [INSERT YOUR FULL NAME]
- Student Number: [INSERT YOUR STUDENT NUMBER]
- Module: Web Development (Introduction) - WEDE5020

## Project Overview
PixelCart Digital Solutions is a (fictional but realistic) business that sells digital
services - web development, social media management, CRM setup, SEO, and branding - as
clear, fixed-price "packages," similar to products in an online store. This repository
contains the website built across the three parts of the WEDE5020 Portfolio of Evidence.

## Website Goals and Objectives
- Generate qualified leads/enquiries for digital service packages.
- Showcase the range of packages clearly, with transparent starting prices.
- Provide an easy way for visitors to request a quote or get in touch.
- KPIs: enquiry form submissions, package page views, average time on services page.

## Key Features and Functionality
- 5-page site: Home, About Us, Services, Enquiry, Contact.
- Consistent header/navigation and footer across all pages, styled with an external
  stylesheet (`css/style.css`) linked from every page.
- Package listings with descriptions, starting prices, and photography.
- Enquiry form with package selection.
- Desktop layout built with CSS Grid and Flexbox (package grid, team grid, hero
  section, nav bar).
- Fully responsive design with two breakpoints (tablet at 1024px, mobile at 600px),
  relative units throughout (rem for type, %/fr/minmax() for widths), and interactive
  states (:hover, :focus-visible, :active) on buttons, links, and cards.
- Responsive images via `srcset`/`sizes` (four width variants per photo: 480w, 800w,
  1200w, 1600w), keeping page weight low on smaller screens.
- (Planned) JavaScript interactivity, custom form validation, and SEO optimisation -
  Part 3.

## Timeline and Milestones
| Part | Focus | Status |
|---|---|---|
| Part 1 | Planning, research, sitemap, HTML structure | Complete |
| Part 2 | CSS styling, responsive design | Complete |
| Part 3 | JavaScript functionality, SEO, forms | Planned |

## Part 1 Details
Part 1 delivers the foundational HTML structure for all 5 pages, a sitemap, an
organised file/folder structure, and the initial project research.

## Part 2 Details
Part 2 implements the full visual design across all 5 pages via one external
stylesheet, `css/style.css`, linked from every page's `<head>`:

- **Base style and design tokens**: colours, fonts, spacing and shadow values are
  defined once as CSS custom properties (`:root`) and reused everywhere, so the whole
  site's look can be changed from one place - this is the "cascading" approach the
  brief asks for, using a minimum number of distinct selectors.
- **Typography**: Poppins for headings and Inter for body text (loaded via Google
  Fonts, with system-font fallbacks), on a type scale from 0.875rem up to 2.441rem.
- **Layout**: Flexbox for the header/nav bar, the homepage hero, and the footer; CSS
  Grid for the services package grid and the About page team grid, using
  `repeat(auto-fit, minmax(...))` so column counts adjust automatically.
- **Visual styling and interactivity**: card shadows, rounded corners, and
  `:hover`/`:focus-visible`/`:active` states on every button, link, and card.
- **Responsive design**: two breakpoints (`max-width: 1024px` for tablet,
  `max-width: 600px` for mobile) switch the package/team grids from 3 columns to 2 to
  1, and stack the navigation on the smallest screens. Relative units (`rem`, `%`,
  `fr`, `minmax()`) mean very little layout code has to change at each breakpoint.
- **Responsive images**: every photo, including the homepage hero, now has four
  generated width variants (480w, 800w, 1200w, 1600w) served via `srcset`/`sizes`,
  so a phone downloads a small file and a desktop downloads a larger one. The
  homepage hero specifically uses a `<picture>` element wrapping the same
  `srcset` pattern.

### Note on Part 1 feedback
At the time Part 2 was completed, marks and lecturer feedback for Part 1 had not yet
been released. No corrections from Part 1 feedback are reflected in this changelog
for that reason - once feedback is received, corrections will be implemented and
logged here as their own dated entries, as the brief requires.

## Sitemap
```
Homepage (index.html)
    |-- About Us (about.html)
    |-- Services (services.html)
    |-- Enquiry (enquiry.html)
    |-- Contact (contact.html)
```
All four pages are reachable from the homepage via the main navigation menu, and each
page links back to every other page through the same shared navigation.

## File/Folder Structure
```
pixelcart/
    index.html
    about.html
    services.html
    enquiry.html
    contact.html
    css/
        style.css
    js/
        script.js
    images/
        hero-photo.jpg (+ -480w/-800w/-1200w/-1600w variants)
        about-team.jpg (+ -480w/-800w/-1200w/-1600w variants)
        package-website.jpg (+ width variants)
        package-social.jpg (+ width variants)
        package-crm.jpg (+ width variants)
        package-seo.jpg (+ width variants)
        package-branding.jpg (+ width variants)
    screenshots/
        index-desktop.png / index-tablet.png / index-mobile.png
        services-desktop.png / services-tablet.png / services-mobile.png
    README.md
```

## Responsive Design Evidence
Screenshots below were taken with the actual stylesheet applied, at three viewport
widths: desktop (1440px), tablet (800px), and mobile (375px). Full-size images are in
the `screenshots/` folder.

**Homepage**
| Desktop | Tablet | Mobile |
|---|---|---|
| ![Homepage desktop](screenshots/index-desktop.png) | ![Homepage tablet](screenshots/index-tablet.png) | ![Homepage mobile](screenshots/index-mobile.png) |

**Services page**
| Desktop | Tablet | Mobile |
|---|---|---|
| ![Services desktop](screenshots/services-desktop.png) | ![Services tablet](screenshots/services-tablet.png) | ![Services mobile](screenshots/services-mobile.png) |

## Changelog
- **[Insert Date]** - Part 1: Initial project structure created. Sitemap, file/folder
  structure, and 5 HTML pages (Home, About, Services, Enquiry, Contact) built with
  semantic HTML5, integrated content, and a shared navigation system. Placeholder
  `style.css` and `script.js` files added for Parts 2 and 3.
- **[Insert Date]** - Part 2: Built the full external stylesheet (`css/style.css`)
  covering design tokens, typography, layout (Flexbox + CSS Grid), visual/interactive
  styling, and responsive design at two breakpoints. Linked Google Fonts (Poppins,
  Inter) from all 5 pages. Generated four responsive width variants for each photo
  and added `srcset`/`sizes` to every `<img>` tag. Added screenshot evidence at
  desktop/tablet/mobile widths for the homepage and services page.
- **[Insert Date]** - Part 2: No Part 1 corrections logged this round - lecturer
  feedback for Part 1 had not yet been released at time of submission.
- **[Insert Date]** - Part 2: Added the real homepage hero photo
  (`images/hero-photo.jpg`, plus responsive width variants), replacing the
  temporary SVG placeholder, and wired it up with a `<picture>` element.

## References
- Anthropic. (2026). *Claude Sonnet 5* [Large language model]. https://claude.ai/
- Negative Space. 2016. Macbook pro showing text. [Online]. Available at:
  https://www.pexels.com/photo/coffee-writing-computer-blogging-34600/ [Accessed
  21 September 2026]. (Used as the homepage hero image, images/hero-photo.jpg.)
- Google Fonts. 2026. Poppins and Inter. [Online]. Available at:
  https://fonts.google.com/ [Accessed 21 September 2026]. (Typeface hosting used for
  all page headings and body text via `css/style.css`.)
- cottonbro studio. 2024. Coding on a laptop. [Online]. Available at:
  https://www.pexels.com/photo/coding-on-a-laptop-5483075/ [Accessed 21 September
  2026]. (Used as the homepage hero image, images/hero-photo.jpg.)
- Edmond Dantès. 2020. People sitting on black leather sofa having a conversation.
  [Online]. Available at: https://www.pexels.com/photo/people-sitting-on-black-leather-sofa-having-a-conversation-4343030/
  [Accessed 21 September 2026]. (Used on the About Us page, images/about-team.jpg.)
- Tranmautritam. 2017. Macbook pro displaying website version 2 on table. [Online].
  Available at: https://www.pexels.com/photo/macbook-pro-displaying-website-version-2-on-table-285814/
  [Accessed 21 September 2026]. (Used for the Website Starter Package,
  images/package-website.jpg.)
- Pixabay. 2026. Facebook application icon. [Online]. Available at:
  https://www.pexels.com/photo/facebook-application-icon-147413/ [Accessed 21
  September 2026]. (Used for the Social Media Management package,
  images/package-social.jpg.)
- Jakub Zerdzicki. 2026. Close-up of programmer typing code on laptop. [Online].
  Available at: https://www.pexels.com/photo/close-up-of-programmer-typing-code-on-laptop-36496927/
  [Accessed 21 September 2026]. (Used for the CRM Setup Package,
  images/package-crm.jpg.)
- cottonbro studio. 2024. Samples of colors. [Online]. Available at:
  https://www.pexels.com/photo/samples-of-colors-6583350/ [Accessed 21 September
  2026]. (Used for the Branding Package, images/package-branding.jpg.)
- AlphaTradeZone. 2024. Close up shot of a computer screen. [Online]. Available
  at: https://www.pexels.com/photo/close-up-shot-of-a-computer-screen-5784807/
  [Accessed 21 September 2026]. (Used for the SEO Boost Package,
  images/package-seo.jpg. Note: the image file's embedded EXIF metadata credits
  a different name, Georgi Georgiev/Georgi Georgiev Photography - the Pexels
  page itself, cited here, credits AlphaTradeZone.)
