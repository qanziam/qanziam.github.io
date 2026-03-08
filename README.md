# QANZIAM Website

**Welcome!** This is the website for QANZIAM, the Queensland branch of ANZIAM (Australian and New Zealand Industrial and Applied Mathematics).

**Everyone has permission to update this website!**
You don't need to ask first, we are delighted you want to help.
Whether you're fixing a typo, adding a seminar, updating committee details, or anything else — your contribution is genuinely appreciated.
You don't need to be an expert, just have a go, and we'll work with you to get it merged.

**You can't break anything.** 
All changes go through a pull request, which gets reviewed before going live. So please don't worry about making mistakes — that's what review is for.

## What can I contribute?

Anything! But here are some ideas:
- Add a new seminar to the [2026 seminars page](seminars/2026/index.html) (there's a ready-made template in the HTML comments)
- Update committee member details or photos
- Fix typos or broken links
- Add a past conference record
- Improve the design or accessibility
- Suggest something new by [opening an Issue](../../issues)

## How the site works

The site is **plain HTML and CSS** — no build step, no frameworks to install, no dependencies. Every `.html` file is exactly what visitors see. We use [Tailwind CSS](https://tailwindcss.com/) via CDN, so you don't need to install anything to make styling changes.

## Site structure

```
index.html                        Main landing page
current-conference.html           This year's conference details
past_conferences/
  index.html                      Conference archive
  conference_2025/index.html      2025 conference page
seminars/
  2025/index.html                 2025 seminars
  2026/index.html                 2026 seminars (has a template in comments)
rules_documents/index.html        Branch rules and annual reports
past_office_bearers.html          Past executive committees
assets/                           Images, logos, and favicons
```

## How to contribute

### Option 1: Edit directly on GitHub (easiest)

1. Navigate to the file you want to change on GitHub
2. Click the pencil icon to edit
3. Make your changes
4. Click **Commit changes**, then **Propose changes**
5. GitHub will create a pull request for you — done!

This is perfect for small changes like adding a seminar, fixing text, or updating a link.

### Option 2: Edit locally (for bigger changes)

1. Fork and clone the repository
2. Make your changes in any text editor
3. Preview in your browser 
    - Easy way: open the HTML file directly. This is enough for quick checks like "Did I put the right text in the seminar entry?"
    - More involved way: run a local server with command:
        ```
        python3 -m http.server 8000 -d .
        ```
        Then visit `http://localhost:8000` to see your changes. This is useful for checking full styling and navigation between pages.
4. Commit, push, and open a pull request

### Not sure how to do any of this?

No worries — just [open an Issue](../../issues) describing what you'd like changed, and someone will take care of it. You can also email [nadiah@nadiah.org](mailto:nadiah@nadiah.org) if you prefer.

## Tips for editing

- **Adding a seminar?** Open `seminars/2026/index.html` and look for the HTML comment near the bottom — it contains a complete template you can copy and fill in.
- **Adding a photo?** Put it in the same directory as the page that uses it. Aim for under 1MB.
- **Changing styles?** We use Tailwind CSS utility classes. The [Tailwind docs](https://tailwindcss.com/docs) are excellent and searchable.
