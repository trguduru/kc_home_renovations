# KC Home Renovations

Static multi-page website for KC Home Renovations — built for [GitHub Pages](https://pages.github.com/).

## Pages

- **Home** (`index.html`) — hero, service highlights, CTA
- **Services** (`services.html`) — kitchens & baths, interior & exterior, full remodels
- **Gallery** (`gallery.html`) — project showcase (add your own photos)
- **About** (`about.html`) — company story and values
- **Contact** (`contact.html`) — contact form and info

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
# Python
python3 -m http.server 8000

# Node (npx)
npx serve .
```

Then visit `http://localhost:8000`.

## Deploy to GitHub Pages

### 1. Create a repo on GitHub

- Go to [github.com/new](https://github.com/new).
- Name it (e.g. `kc_home_renovations`).
- Choose **Public**, then **Create repository** (do not add a README or .gitignore if the project already has files).

### 2. Push this folder to GitHub

From the project folder in your terminal:

```bash
cd /path/to/kc_home_renovations   # your project folder

git init
git add .
git commit -m "Initial commit: KC Home Renovations site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/kc_home_renovations.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username and `kc_home_renovations` with your repo name if different.

### 3. Turn on GitHub Pages

- Open your repo on GitHub → **Settings** → **Pages** (left sidebar).
- Under **Source**, choose **Deploy from a branch**.
- **Branch:** `main` (or `master`) → **Folder:** `/ (root)` → **Save**.

### 4. Wait and open your site

- GitHub builds the site in 1–2 minutes.
- Your site will be at: **`https://YOUR_USERNAME.github.io/kc_home_renovations/`**

The `.nojekyll` file tells GitHub Pages to serve the files as-is (no Jekyll build).

## Contact form

The contact form is static HTML. To receive submissions, use a form service (e.g. [Formspree](https://formspree.io/)) and set the form `action` to their endpoint, or host the site with a provider that supports serverless forms.
