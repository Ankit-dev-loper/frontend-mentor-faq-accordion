[![Releases · Download](https://img.shields.io/badge/Releases-Download-blue?logo=github&style=for-the-badge)](https://github.com/Ankit-dev-loper/frontend-mentor-faq-accordion/releases)

# Responsive FAQ Accordion — HTML, CSS & JavaScript Component

An interactive, responsive FAQ accordion built for the Frontend Mentor challenge. The component uses semantic HTML, modern CSS, and vanilla JavaScript. It focuses on accessibility, performance, and a small footprint so you can reuse it in real projects.

🧩 Live demo: responsive accordion UI  
🎯 Built for Frontend Mentor challenge  
⚡ Fast, accessible, theme-aware

---

![FAQ Accordion Preview](https://images.unsplash.com/photo-1526318472351-c75fcf0703f8?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=60)

Table of contents
- About
- Demo and Releases
- Features
- Design and accessibility
- Tech stack
- Getting started
- Usage
- Theme toggle
- Development tips
- Performance and Lighthouse
- Deployment (Netlify)
- Git, GitHub and workflow
- Testing and QA
- Contributing
- License
- Authors and credits
- Changelog and releases

About
This repo contains a production-ready FAQ accordion. It implements an accessible accordion pattern with keyboard support, ARIA attributes, and reduced motion support. Use it as a component in a static page or as part of a larger UI.

Demo and Releases
Start here:
https://github.com/Ankit-dev-loper/frontend-mentor-faq-accordion/releases

Use the Releases page to grab packaged builds. Download the latest release asset (zip or tarball), extract it, and open the index.html file in your browser to run the project locally. The releases include prebuilt CSS and a ready-to-run index.html so you can test the UI fast.

If the Releases page does not show assets for your environment, check the "Releases" section on the repository for tagged builds and changelogs:
https://github.com/Ankit-dev-loper/frontend-mentor-faq-accordion/releases

Features
- Semantic HTML structure for content and headings.
- Custom, theme-aware CSS with a light/dark toggle.
- Pure JavaScript accordion logic without frameworks.
- Smooth open/close transitions using CSS height animation.
- Keyboard navigation: Tab and Arrow keys, Home/End support.
- ARIA attributes for expanded/collapsed state and roles.
- Reduced-motion support via prefers-reduced-motion.
- Small bundle size and no external runtime dependencies.
- Cross-browser support for modern browsers.

Design and accessibility
The accordion follows accessible UI patterns:
- Buttons have aria-controls and aria-expanded.
- Panels use role="region" and aria-labelledby.
- Keyboard users can move focus with Arrow keys.
- The design uses high-contrast color tokens and clear hit targets.
- Motion respects prefers-reduced-motion.

The layout adapts to narrow screens. The FAQ list stacks vertically on phones. On wider screens, the container centers with a max-width for legibility.

Tech stack
- HTML5 (semantic)
- CSS3 (variables, flexbox, transitions)
- JavaScript (ES6 modules, no build step)
- Optional: Netlify for deploy preview
Topics: 5th-month, accordion, css, frontend-mentor, git, github, html, javascript, lighthouse, netlify, perfectpixel, project, theme-toggle, vscode

Getting started
You can run the project locally with two approaches.

Option A — Download release (no build)
1. Visit Releases: https://github.com/Ankit-dev-loper/frontend-mentor-faq-accordion/releases  
2. Download the latest release zip.  
3. Extract the zip.  
4. Open index.html in your browser.

Option B — Clone and run locally (dev)
1. git clone https://github.com/Ankit-dev-loper/frontend-mentor-faq-accordion.git  
2. cd frontend-mentor-faq-accordion  
3. Open index.html in your browser or run a static server:
   - Python 3: python -m http.server 8000
   - Node (http-server): npx http-server -c-1

Usage
- The HTML contains a list of question items. Each question is a button element. Each answer is a panel element.
- Toggle a question by clicking the button or pressing Enter/Space.
- Use ArrowUp and ArrowDown to move between buttons.
- Use Home and End to jump to first and last items.
- The theme toggle stores preference in localStorage so the page remembers your choice.

Markup example (excerpt)
- A question uses <button aria-expanded="false" aria-controls="faq-1">.
- The associated panel uses id="faq-1" role="region" aria-labelledby="btn-faq-1".

Theme toggle
The project includes a simple theme toggle. It toggles a data-theme attribute on the root element and stores the choice in localStorage.

Implementation notes:
- CSS variables drive color tokens.
- The JS reads initial preference from localStorage or prefers-color-scheme.
- Toggle works without a page reload.

Development tips
- Use the component as a partial or include in templates.
- The CSS uses CSS variables. Override the variables in a root stylesheet to match your site.
- Keep transitions on max-height or transform where possible. The component uses a measured height technique to animate the panel.
- To add new items, copy the markup for one question and update ids and aria-controls.

VSCode tips
- Enable editor.formatOnSave for consistent formatting.
- Use the Emmet abbreviation for quick HTML scaffolding.
- Add the workspace setting "files.associations": {"*.css": "css"} for proper highlighting.

Performance and Lighthouse
The component keeps assets minimal:
- No external frameworks reduce parse time.
- CSS and JS are small and served without runtime.
- The markup is semantic and speeds indexability.
- Use preconnect if you add external fonts.
- Run Lighthouse audits to verify accessibility and performance scores. The project targets a high Lighthouse score by default.

Testing and QA
- Manual testing: keyboard navigation, screen reader check (NVDA / VoiceOver), responsive layout on mobile.
- Automated checks: run axe or Lighthouse CI in your pipeline.
- Visual checks: use PerfectPixel or pixel-diff tools if you enforce a visual spec.

Deploying (Netlify)
- This project works as a static site.
- Connect the repo to Netlify or drag-and-drop the built folder (the extracted release).
- Set the publish directory to the root where index.html lives.
- Netlify supports previews for PRs and automatic deploys on push.

Git, GitHub and workflow
- Branch strategy: use feature branches and open Pull Requests.
- Keep commits focused and atomic.
- Use PR templates to include testing steps and screenshots.
- Tag releases with semantic version numbers (v1.0.0) and publish assets on the Releases page.

Testing checklist before PR:
- Run accessibility checks.
- Validate keyboard interactions.
- Check theme toggle persistence.
- Ensure no console errors in the browser.

Contributing
- Fork the repo and create a branch per change.
- Open a PR against main with a clear changelog entry.
- Include a screenshot or animated GIF for UI changes.
- Keep the scope small so reviews run fast.

License
This project uses the MIT license. See LICENSE file for full text.

Authors and credits
- Creator: Ankit-dev-loper (Frontend Mentor build)
- Challenge: Frontend Mentor — FAQ Accordion
- Icons and images: Unsplash and open-source icon sets

Changelog and releases
See the Releases page for packaged builds, version notes, and downloadable assets:
https://github.com/Ankit-dev-loper/frontend-mentor-faq-accordion/releases

From the Releases page, download the asset for the release you want. After download, extract the archive and run index.html to load the component in your browser. Release assets typically contain:
- index.html
- css/
- js/
- assets/

Acknowledgments
- Frontend Mentor for the challenge and mockup.
- Community contributors for pattern guidance.
- Open-source tools for dev ergonomics.

Badges and quick links
[![Release · Download](https://img.shields.io/badge/Releases-Visit%20Releases-brightgreen?logo=github)](https://github.com/Ankit-dev-loper/frontend-mentor-faq-accordion/releases)
- Repo: https://github.com/Ankit-dev-loper/frontend-mentor-faq-accordion
- Releases: https://github.com/Ankit-dev-loper/frontend-mentor-faq-accordion/releases

How to cite or reuse
- Drop the HTML snippet into your page.
- Link the CSS; include the JS before closing body tag.
- Keep role and aria attributes for accessibility.

Common issues
- If the panel animation stutters, check for layout thrash caused by DOM writes inside the animation loop.
- If keyboard focus jumps, ensure focus is not being programmatically moved unless needed.
- If theme does not persist, verify localStorage permissions in the browser.

Files you will find
- index.html — demo and markup
- src/css/styles.css — main styles (or dist css in release)
- src/js/main.js — accordion behavior and theme toggle
- assets/ — images and icons
- LICENSE, README.md, CONTRIBUTING.md

Contact
Open an issue or PR on the repository for bugs, questions, or feature requests. Use clear steps to reproduce and include your browser and OS.

End of file.