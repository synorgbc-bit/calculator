# Oligonucleotide Molecular Weight Calculator

A single-page, client-side calculator for IDT-style oligonucleotide sequences. It parses DNA/RNA/2′-OMe/LNA bases, `/code/` modifications, and phosphorothioate linkages, then reports average molecular weight with an optional per-token breakdown.

## Use locally
1. Clone the repository:
   ```bash
   git clone <your-repo-url>.git
   cd calculator
   ```
2. Open `index.html` directly in your browser (no build or server needed). Double-click the file or run:
   ```bash
   xdg-open index.html  # Linux
   open index.html      # macOS
   start index.html     # Windows
   ```
3. Paste an IDT-style sequence, adjust mass tables/deltas as needed, and read the calculated MW and breakdown.

## Quick free hosting (GitHub Pages)
A ready-made GitHub Actions workflow is included. To publish your live calculator:

1. Push this repository to GitHub (keep the default branch named `main` or update the workflow trigger accordingly).
2. In GitHub, go to **Settings → Pages** and set **Source** to **GitHub Actions**.
3. Under **Environments**, approve the **github-pages** environment if prompted.
4. Push to `main` (or use **Actions → Deploy to GitHub Pages → Run workflow**) to build and deploy. The page will publish at `https://<your-username>.github.io/<repo-name>/`.
5. Future pushes to `main` auto-deploy via the workflow at `.github/workflows/deploy-pages.yml`.

If you prefer the older "Deploy from a branch" method, you can still use it by choosing the branch and `/ (root)` folder in **Settings → Pages**, but the included workflow is recommended for cleaner, automatic deploys.

## Alternative free hosting options
If you prefer, services like Netlify or Vercel also work: drag-and-drop `index.html`, or connect your repo for auto-deploys. No configuration beyond static hosting is needed.
