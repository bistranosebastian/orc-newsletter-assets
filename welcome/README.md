# ORC welcome email (newsletter confirmation)

Goes in the `orc-newsletter-assets` repo as the `welcome/` folder (repo root).
Images are referenced from:
https://cdn.jsdelivr.net/gh/bistranosebastian/orc-newsletter-assets@main/welcome/<file>

After pushing: pin `@main` to the commit hash in welcome-email.html so jsDelivr never serves stale files.

- welcome-email.html: final email HTML (Brevo transactional template, sender Echipa ORC <run@>)
- Greeting uses Brevo logic: Salut{% if contact.FIRSTNAME %}, {{ contact.FIRSTNAME }}{% endif %}!
- Mobile: fluid 600px container, stacks under 620px. Dark mode: prefers-color-scheme + Outlook [data-ogsc]/[data-ogsb] rules.
- Rounded corners and circles are baked into the PNGs (Gmail/Outlook ignore some CSS radius).
- Design reference for restyling the monthly newsletter: Castoro (headings, italic accents) + Nunito, cream #FCFAF7 / #F3EEE6, indigo #252158, coral #EE4947, ink #0D0503, text #1E2945.
