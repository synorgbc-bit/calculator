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
You can serve this static HTML directly from your repo with GitHub Pages:

1. Commit and push the latest changes to your GitHub repository.
2. In the GitHub UI, go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**.
4. Select the branch you want to publish (e.g., `main`) and folder `/ (root)`.
5. Save. GitHub will publish your site at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

Updates are automatic—whenever you push changes to the published branch, the live page refreshes.

## Alternative free hosting options
If you prefer, services like Netlify or Vercel also work: drag-and-drop `index.html`, or connect your repo for auto-deploys. No configuration beyond static hosting is needed.
