Roots of Hope Foundation Website

Project overview

Roots of Hope Foundation is a responsive, accessible community-organisation website. The single-page HTML project uses JavaScript page routing to present the Home, About Us, Programmes, Get Involved, and Contact sections through a shared navigation bar and footer.

 Files

| File | Purpose |
|---|---|
| `roots-of-hope-website_15.html` | Main HTML document containing the website content, forms, navigation, page sections, and JavaScript interactions. |
| `style.css` | External stylesheet for the complete visual design, desktop layout, responsive breakpoints, forms, cards, navigation, and accessibility states. |
| `screenshots/` | Desktop, tablet, and mobile viewport evidence for Part 2 testing. |

 Part 2 implementation

 External stylesheet

The HTML file links to the external stylesheet with the following declaration:

```html
<link rel="stylesheet" href="style.css">
```

The stylesheet uses consistent class naming, CSS custom properties, a reset, and reusable component rules rather than repeating declarations unnecessarily.

 Base and typography styles

The stylesheet establishes a warm, nature-inspired colour palette using CSS custom properties. It defines Montserrat for headings, Open Sans for body copy and controls, and Lora for quotation text. Font sizes use `rem` and `clamp()` where appropriate, with consistent line-height, font-weight, and letter-spacing rules.

 Desktop layout

The desktop solution uses CSS Grid for programme cards, team cards, mission and vision cards, contact content, maps, statistics, and programme details. Flexbox is used for navigation, buttons, social links, radio controls, and footer links. Cards use borders, rounded corners, shadows, hover movement, and consistent spacing.

 Responsive design

The layout includes tablet rules at `64rem` and mobile rules at `48rem`. Multi-column layouts collapse to one column on small screens. The navigation becomes a toggleable mobile menu using the existing JavaScript. Hero buttons become full-width on mobile, headings scale with `clamp()`, and maps, forms, cards, and content sections adapt to narrow viewports.

Relative units used include `rem`, `%`, `min()`, `max()`, and `clamp()`. Images use `max-width: 100%` and `object-fit` rules to prevent overflow. Keyboard focus styles are visible for links, buttons, and form controls.

 Testing and evidence

The website was checked locally using Chromium at the following viewport sizes:

| Viewport | Purpose | Evidence |
|---|---|---|
| 1440 × 1000 | Desktop layout | `screenshots/desktop-home.png` |
| 1024 × 1000 | Tablet layout | `screenshots/tablet-home.png` |
| 390 × 844 | Mobile layout | `screenshots/mobile-home.png` |

The following interactions should also be tested in the browser before submission:

1. Select each navigation link and confirm that the matching page section appears.
2. Resize the browser below the mobile breakpoint and open and close the navigation toggle.
3. Select the Volunteer and Sponsor enquiry options and confirm that the relevant conditional fields appear.
4. Submit each form and confirm that the demonstration confirmation alert appears and the form resets.
5. Check that keyboard focus is visible when tabbing through navigation, buttons, links, and form controls.
6. Confirm that the two map iframes load and that no horizontal scrolling appears at mobile width.

 Changelog

 Part 2 — CSS styling and responsive design

- Created the complete external stylesheet `style.css` and matched the HTML link reference.
- Added a cross-browser CSS reset and centralised design tokens for colours, typography, spacing, borders, radii, and shadows.
- Added shared navigation styling, active-link states, sticky positioning, and a responsive mobile menu presentation.
- Added page-routing visibility rules so `.page` sections are hidden by default and `.page.active` is displayed.
- Added desktop Grid and Flexbox layouts for the hero, programme cards, statistics, mission and vision cards, team cards, forms, contact information, and maps.
- Added visual styling for cards, buttons, calls to action, forms, map panels, footer links, borders, and shadows.
- Added hover states and visible keyboard focus states to support usability and accessibility.
- Added tablet and mobile media queries using relative units and responsive column changes.
- Added reduced-motion and print rules.
- Added `README.md` documentation covering the Part 2 implementation, testing plan, evidence, changelog, and references.

 Part 1 feedback corrections

- Consolidated the visual presentation into one external stylesheet rather than relying on inline page styling.
- Preserved the existing semantic HTML structure, labels, form associations, navigation attributes, page headings, and accessible map titles.
- Added layout rules for all existing HTML component classes so the content is consistently styled across the routed page sections.

 References

- MDN Web Docs. *CSS media queries*. https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries
- MDN Web Docs. *CSS Grid Layout*. https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout
- MDN Web Docs. *Using media queries for responsive design*. https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries/Using_media_queries
- MDN Web Docs. *:focus-visible*. https://developer.mozilla.org/en-US/docs/Web/CSS/:focus-visible
- Google Fonts. *Montserrat, Open Sans, and Lora*. https://fonts.google.com/

 Submission checklist

- [x] HTML file included.
- [x] External `style.css` included and linked.
- [x] Desktop, tablet, and mobile screenshot evidence included.
- [x] README includes Part 2 explanation and changelog.
- [x] README includes references.
- [ ] Commit the final files with descriptive Git messages.
- [ ] Push the final files to the GitHub repository.
- [ ] Open the remote repository in a browser and verify that the submitted files and screenshots are visible.
- [ ] Submit the working GitHub repository link through the LMS.
