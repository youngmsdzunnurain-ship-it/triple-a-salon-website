# Triple A Salon Website

A responsive, static website for Triple A Salon in Gwagwalada, Abuja.

## Project structure

```
.
├── index.html
├── css/
│   └── style.css
├── js/
│   └── script.js
├── assets/
│   └── images/
│       └── triple-a-logo.png
└── README.md
```

## Features

- Responsive salon landing page and services list
- Haircut gallery with African/Nigerian barbershop photography references
- Visible barbershop hero photograph and real barber-tools/clipper feature image
- WhatsApp contact and appointment-message handoff
- Email contact link (configure the salon email in `js/script.js`)
- No database, server-side application, or backend required

## Contact configuration

In `js/script.js`, update:
- `PHONE`: WhatsApp number in international format without the plus sign
- `SHOWN`: human-readable phone number
- `EMAIL`: salon email address (leave empty until the confirmed address is available)

## Run locally

This is a static site. Open `index.html` directly, or run a local preview:

```sh
php -S 127.0.0.1:8086
```

Then visit http://127.0.0.1:8086.

## Photography

Gallery photos are served from Pexels CDN URLs. Their individual source pages and free-use status should be retained when replacing or changing images:
- https://www.pexels.com/photo/barber-giving-haircut-in-traditional-shop-33418521/
- https://www.pexels.com/photo/barbershop-haircut-for-black-male-client-35157692/
- https://www.pexels.com/photo/a-man-in-a-barbershop-7697228/
- https://www.pexels.com/photo/close-up-of-black-man-holding-haircut-tool-7697396/
- https://www.pexels.com/photo/man-getting-his-hair-trimmed-7447150/

Images should be replaced with the salon's own client photos when available and consent has been obtained.


## Search engine and launch readiness

The page includes a descriptive title and meta description, Open Graph/Twitter sharing metadata, structured local business information (JSON-LD), and a basic `robots.txt`.

Before launch on a public domain:
- Set the canonical URL and add a sitemap using the final HTTPS domain.
- Verify the domain in Google Search Console and submit the sitemap.
- Add a final social-sharing image with appropriate rights and descriptive alt text.
- Test all navigation, contact actions, image loading, and downloads on mobile and desktop.

Search engines decide when and whether to index a site; metadata improves clarity but does not guarantee ranking or immediate appearance in results.


## Privacy and accessibility
A privacy notice is available at `privacy.html`. Booking details are passed to WhatsApp only when the visitor chooses to submit; this static website does not store bookings. Booking fields have visible labels and gallery images load lazily with alternative text.
