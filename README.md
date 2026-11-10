# Lantern Row Market

An events website built on [Total CMS](https://totalcms.co), for a Friday night street market with news, a season of events and a contact form. Every page is filled with demo content, so the site works as soon as it's installed. It's the finished site from the Total CMS beginner videos, so it's also a good site to learn from.

## What's in it

- **News:** posts with a page each, a cover photo and a photo gallery
- **Events:** each one with a date, a location, a poster and a schedule. The Events page shows only upcoming events, soonest first, and hides them once they've passed
- **Contact form:** public, protected from bots, and saved in the admin. It sends visitors to a thank-you page
- **Colors in the admin:** four objects in the Color collection set the site's colors, so you can change them without touching CSS
- **One stylesheet:** plain CSS with no build step, in `public/assets/market/market.css`

## Install

With Composer:

```bash
composer create-project totalcms/starter-events mysite
```

Point your web server's document root at `mysite/public/`, then visit the site. The setup wizard creates your admin account. Then open `/readme` on the site for a tour and a list of what to change before launch.

## Make it yours

- **Content.** Sign in at `/admin` to edit the posts, events and photos.
- **Colors.** Open the **Color** collection and change `paper`, `paper-deep`, `ink` or `lantern`. The site follows on the next page load.
- **Templates.** The layout and page templates are in **Builder** in the admin, and in `tcms-data/builder/` on disk. The footer's hours, email and phone are in the `default` layout.
- **Fonts and spacing.** These are at the top of `public/assets/market/market.css`. It styles plain HTML, so the templates stay short.

## Photos

The demo photos come from Pexels, and `CREDITS.md` credits each photographer. Replace them with your own before the site goes live.

## Going live

Change the hours, email and phone in the footer of the `default` layout, and delete the `/readme` page. Contact form messages are saved in the admin under **Contact**. They aren't emailed.

## Requirements

PHP 8.2 or later, and a Total CMS Pro license for the domain you deploy to. The site uses custom schemas for its events and contact form. It runs free, with every feature, on a local development domain such as `mysite.test`.
