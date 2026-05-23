# Portfolio — GitHub Pages Template

Modelled on the layout of [briannahuxtable.com](https://briannahuxtable.com):
clean nav → hero intro → alternating project cards → project detail pages → about page.

---

## File structure

```
portfolio/
├── index.html          ← Work / home page
├── about.html          ← About page
├── project-1.html      ← Project detail (duplicate for each project)
├── css/
│   └── style.css       ← All styles; design tokens at the top
├── js/
│   └── main.js         ← Nav scroll, burger menu, scroll animations
└── images/             ← Drop your images here
    ├── project-1.jpg
    ├── project-2.jpg
    ├── project-3.jpg
    └── me.jpg
```

---

## Quickstart

### 1. Find & replace "Your Name"
Search the whole folder for `Your Name` and replace with your actual name.

### 2. Customise the design tokens
Open `css/style.css` and edit the `:root` block at the top:
- `--color-accent` — your highlight colour (links, tags, buttons)
- `--color-bg` — page background
- `--color-text` — body text
- `--font-display` / `--font-body` — swap Google Fonts to any pairing you like

### 3. Edit `index.html`
- Update `.hero__tagline` and `.hero__role`
- For each project, edit the `.project-card` blocks:
  - `project-card__tag` — platform/type label
  - `project-card__company` — company or academic context
  - `project-card__title` — project name
  - `project-card__desc` — 1–2 sentence description
  - Link `href` to the matching `project-X.html`
  - `<img src>` — point at your image in `/images/`

### 4. Edit `about.html`
- Update bio paragraphs
- Add a photo as `images/me.jpg` (square crop works best)
- Update the email link

### 5. Duplicate `project-1.html` for each project
- Save as `project-2.html`, `project-3.html`, etc.
- Fill in the hero metadata, body sections, and images
- For NDA projects, use the email CTA variant shown in `index.html`

### 6. Add your images
Drop files into `/images/`. Recommended sizes:
- Project card covers: **1200 × 900 px** (4:3 ratio)
- Project detail images: **1400 × 900 px** or wider
- About photo: **600 × 600 px** minimum, square crop

### 7. Update footer links
In all HTML files, find the `<footer>` and update:
- LinkedIn URL
- Email address
- Any additional links (GitHub, Dribbble, etc.)

---

## Deploying to GitHub Pages

1. Create a repo named `yourusername.github.io`
2. Push this folder's contents to the `main` branch (not inside a subfolder)
3. Go to **Settings → Pages → Source → Deploy from branch → main / root**
4. Your site will be live at `https://yourusername.github.io` within a minute

### Custom domain (optional)
Add a file named `CNAME` at the root containing just your domain:
```
yourname.com
```
Then point your domain's DNS to GitHub Pages IPs.

---

## Adding more pages
1. Duplicate `project-1.html`
2. Add a new `.project-card` in `index.html` pointing to it
3. No build step required — it's plain HTML/CSS/JS

---

## Fonts
Currently using [Playfair Display + DM Sans](https://fonts.google.com/) from Google Fonts.
To swap, replace the `<link>` tag in each HTML file and update `--font-display` / `--font-body` in the CSS.

---

*Template built to mirror the structure of briannahuxtable.com — layout and component patterns only, no original content or styles copied.*
