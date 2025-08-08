AR Marker Infographic Demo

Files:
- index.html : single-file demo using A-Frame + AR.js (marker-based)
- README.md : this file

How to test locally (quick):
1. Save `index.html` to a folder.
2. You MUST serve it over HTTPS or at least via localhost (some browsers disallow camera on file://).
   Quick local server (Python 3):
     cd <folder-with-index.html>
     python -m http.server 8000
   Then open http://localhost:8000 in your browser (mobile or desktop).
3. Allow camera access when prompted. Show the Hiro marker to your camera:
   https://raw.githubusercontent.com/AR-js-org/AR.js/master/three.js/examples/marker-training/examples/hiro.png
   (print it or show it on another screen)

Recommended deployment (two options):

A) GitHub Pages (fast, free)
1. Create a new repo on GitHub and push the files.
2. In repo settings -> Pages -> choose branch `main` and folder `/ (root)` -> Save.
3. Visit the provided https://<your-username>.github.io/<repo>/ URL.

B) Netlify (drag & drop or git-linked)
1. Create a Netlify account, drag-and-drop the folder containing index.html to Sites -> New site from deploy.
2. Netlify will serve it over HTTPS automatically.

Notes & next steps:
- To use a custom marker-pattern, see AR.js marker training docs: https://ar-js-org.github.io/AR.js-Docs/marker-training/
- To anchor HTML overlays that stay crisp read about `aframe-html-shader` or use CSS-based overlays that are toggled on markerFound.
- If you want, I can adapt this into a React/Next.js page, or deploy it for you (you'd need to grant repo access or upload to a host).
