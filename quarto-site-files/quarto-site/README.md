# zahidasghar.com — Quarto Website

This is the source for [zahidasghar.com](https://zahidasghar.com), built with [Quarto](https://quarto.org/).

## Quick Start — How to Render and Deploy

### Prerequisites

1. **Install Quarto** (if not already installed):
   - Download from [quarto.org/docs/get-started](https://quarto.org/docs/get-started/)
   - Or if you have RStudio 2022.07+, Quarto is already included

2. **Install R** (optional, only needed if you add R code chunks to posts)

### Step 1: Add Your Profile Photo

Replace the placeholder image:

```
images/profile.jpg   ← Replace with your actual headshot (400×500px recommended)
```

### Step 2: Preview Locally

Open a terminal in this project folder and run:

```bash
quarto preview
```

This opens a live preview at `http://localhost:4200`. Any changes you save will auto-refresh.

### Step 3: Render the Site

```bash
quarto render
```

This generates the full site into the `docs/` folder.

### Step 4: Deploy to GitHub Pages

**Option A — Publish directly (recommended):**

```bash
quarto publish gh-pages
```

This creates a `gh-pages` branch and pushes the rendered site. GitHub Pages will serve it automatically.

**Option B — Manual deploy via `docs/` folder:**

1. Push the entire repo (including `docs/`) to your `zahedasghar.github.io` repository
2. In GitHub repo Settings → Pages → set source to "Deploy from a branch" → `main` branch → `/docs` folder
3. Set custom domain to `zahidasghar.com`

### Step 5: Configure Custom Domain

1. In your GitHub repo, go to Settings → Pages → Custom domain → enter `zahidasghar.com`
2. Ensure your DNS has a CNAME record pointing `zahidasghar.com` to `zahedasghar.github.io`
3. The CNAME file will be auto-created by GitHub

## Site Structure

```
.
├── _quarto.yml          # Site configuration (navbar, footer, theme)
├── custom.scss          # Custom theme colors and typography
├── styles.css           # Additional CSS overrides
├── index.qmd            # Homepage
├── about.qmd            # Leadership profile
├── research.qmd         # Publications by theme
├── policy.qmd           # Policy essays and commentary
├── teaching.qmd         # Courses, workshops, R materials
├── code.qmd             # GitHub repos and data projects
├── blog.qmd             # Blog listing page
├── posts/               # Blog posts (each in its own folder)
│   ├── pakistan-ai-policy/
│   │   └── index.qmd
│   └── welcome/
│       └── index.qmd
├── images/
│   └── profile.jpg      # Your headshot
└── README.md
```

## How to Add a New Blog Post

1. Create a new folder under `posts/`:
   ```
   posts/my-new-post/index.qmd
   ```

2. Add YAML front matter:
   ```yaml
   ---
   title: "My New Post Title"
   description: "A brief description for the listing."
   author: "Zahid Asghar"
   date: "2026-03-01"
   categories: [Economics, R, Policy]
   ---
   ```

3. Write your content in Markdown below the YAML

4. Preview with `quarto preview`, then publish with `quarto publish gh-pages`

## How to Add Your CV

Place your CV PDF in the root directory as `cv.pdf`. The About page already links to it.

## Customization

- **Colors**: Edit `$primary` in `custom.scss` (currently navy `#1B4F72`)
- **Fonts**: Edit `$headings-font-family` and `$font-family-sans-serif` in `custom.scss`
- **Navigation**: Edit the `navbar` section in `_quarto.yml`
- **Footer**: Edit `page-footer` in `_quarto.yml`
- **Google Analytics**: Uncomment and add your GA4 ID in `_quarto.yml`
- **Open Graph / Twitter Cards**: Uncomment after adding your profile photo

## After First Deploy — Next Steps

1. Replace placeholder profile photo with your actual headshot
2. Add your CV as `cv.pdf`
3. Uncomment Google Analytics, Open Graph, and Twitter Card configs in `_quarto.yml`
4. Register with Google Search Console for SEO monitoring
5. Start writing blog posts following the 6-month content roadmap
