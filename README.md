# Ashar | Portfolio

Personal portfolio for Ashar, Gold Coast. Cisco CCNA, TAFE Diploma of Information Technology (Advanced Networking and Cloud Engineering), aiming for a junior network engineer role.

**Live site:** https://ashar-networks.github.io

## What is on the site
- Hero console that answers Cisco-style commands (`show vlan brief`, `ping ashar`, `github`, `resume`)
- Skills laid out on the OSI stack
- Router-on-a-stick animation and a VLSM subnet sizer
- Projects, certifications and an experience traceroute
- Resume viewer, download and an ink-friendly print version
- Light and dark mode (dark by default)

## Files
| File | Purpose |
| --- | --- |
| `index.html` | The whole site: HTML, CSS and JavaScript in one file |
| `Ashar-Resume.pdf` | Resume, dark version |
| `Ashar-Resume-Ink-Friendly.pdf` | Resume, light version for printing |
| `resume-page.png`, `resume-page-light.png` | Page previews shown in the on-site resume viewer |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Run it locally
Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Deploy on GitHub Pages
1. Name this repository exactly `ashar-networks.github.io`.
2. Upload all the files above to the root of the `main` branch.
3. Go to **Settings > Pages**, set **Source** to **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. The site goes live at https://ashar-networks.github.io within a couple of minutes.

## Settings in `index.html`
Near the top of the script there is a small settings block:

| Setting | What it does |
| --- | --- |
| `FORM_ENDPOINT` | A Formspree address (`https://formspree.io/f/xxxxxxxx`). Messages from the contact form are forwarded to your inbox. Free plan is fine. |
| `CONTACT_EMAIL` | Used if there is no endpoint. The form then opens the visitor's email app with the message filled in. |
| `PUBLIC_EMAIL` | Optional. Shows your address with a copy button beside the resume buttons. |

If none of these are set, the form shows a "Copy message" button instead, so nothing is lost.

## Updating the resume
Replace the two PDFs and the two PNG previews (the PNGs are the PDFs rendered at 200 dpi), then commit.

## Licence
Content is mine. Please ask before reusing it.
