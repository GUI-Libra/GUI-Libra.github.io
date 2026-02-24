# GUI-Libra Project Website — Template 1 (Dark)

Project website for **GUI-Libra: Training Native GUI Agents to Reason and Act with Action-aware Supervision and Partially Verifiable RL**.

> **Compare templates:** See `../gui-libra-website-v2/` for an alternative light/premium design.

## How to Visualize the Website

### Option 1: Open directly in browser (simplest)

```bash
open index.html
```

Or double-click `index.html` in Finder. Works for local preview, but some features (e.g. external fonts) may load from the network.

### Option 2: Python HTTP server (recommended for development)

```bash
cd gui-libra-website
python3 -m http.server 8000
```

Then open **http://localhost:8000** in your browser.

### Option 3: Node.js / npx

```bash
cd gui-libra-website
npx serve .
```

Then open the URL shown (typically http://localhost:3000).

### Option 4: Deploy to GitHub Pages

1. Create a repo named `GUI-Libra.github.io` (or `your-username.github.io` for a user site)
2. Push the website files to the repo
3. Enable GitHub Pages in repo Settings → Pages → Source: main branch
4. Site will be live at `https://GUI-Libra.github.io`

## Project Structure

```
gui-libra-website/
├── index.html      # Main page
├── assets/
│   ├── overview.png   # Figure 1 from paper (extracted from PDF)
│   └── page_2.png     # Additional figure
└── README.md
```

## Customization

- **Paper link**: Update the "Paper (PDF)" button href when the paper is published
- **arXiv link**: Add the arXiv ID when available
- **Overview figure**: Replace `assets/overview.png` with a high-res export of Figure 1 from the paper for better quality
- **Authors**: Add personal/homepage links in the authors section
