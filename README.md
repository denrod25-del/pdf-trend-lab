# PDF Trend Lab

A free, in-browser tool that pulls numbers out of a PDF (or pasted / CSV data)
and turns them into trend charts. Everything runs client-side — files never
leave the visitor's device.

- **Live site:** https://pdftrendlabapp.com/
- **Stack:** a single static `index.html` (no build step). PDF text extraction
  uses Mozilla's pdf.js loaded from a CDN at runtime; charting and the paste/CSV
  path work fully offline.

## Deploy (GitHub Pages)
1. Push these files to the default branch.
2. Repo → Settings → Pages → Source = default branch, `/` (root).
3. The `CNAME` file claims `pdftrendlabapp.com`; point DNS at GitHub Pages
   (apex `A`/`ALIAS` records + `www` CNAME → `<user>.github.io`).
