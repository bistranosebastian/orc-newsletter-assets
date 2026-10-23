# Povestea Lunii, monthly template

`povestea-lunii-template.html` is the monthly newsletter rebuilt on the same code and design system as `welcome/welcome-email.html`, filled with the September 2026 edition as a working example.

Design: Castoro (headings, italic accents) + Nunito, cream #FCFAF7 / #F3EEE6, indigo #252158, coral #EE4947, ink #0D0503, text #1E2945.

What changed compared with the September send:
- Fluid 600px layout with the Gmail-app fixes, so it no longer overflows in apps that ignore styles.
- Hero is a normal image under the title instead of a CSS background image (Gmail apps with non-Gmail accounts and some Outlooks drop background images).
- Coral labels, numbered list (01 to 03) and dividers from the welcome email, with the lighter coral in dark mode.
- All image URLs pinned to a commit hash instead of @main.
- "Preferințe" link removed to match the welcome email.

Each month:
1. Upload the month's images to `/{yyyy-mm}/` and push.
2. Copy the template, replace the month's image URLs with `@<new commit hash>/{yyyy-mm}/`, and change `utm_campaign=newsletter_yyyy_mm`.
3. Update every block marked `EDIT:` (title, preheader, footer line for the partners list).
4. Create the Brevo campaign from the file via htmlUrl.
