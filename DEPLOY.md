# Deploy TechBunny.ai

Static site. `index.html` at the root, images in `/assets`. Works on any static host.

## Option 1: Netlify Drop (fastest, free)
1. Unzip this folder.
2. Go to https://app.netlify.com/drop
3. Drag the whole unzipped folder (the one containing index.html) onto the page.
4. You get a public URL in seconds. Add a custom domain later if you want.

## Option 2: GitHub Pages
1. Create a repo and add these files at the root (keep the assets folder).
2. Settings, then Pages, then Source: deploy from a branch, root.
3. The site goes live at the Pages URL.

## Option 3: AWS S3 + CloudFront (production)
1. Create an S3 bucket. Upload index.html and the assets folder, keeping the paths.
2. Enable static website hosting and set index.html as the index document.
3. Put CloudFront in front for HTTPS and caching. Point your domain with Route 53.

## Notes
- Fonts load from Google Fonts (needs internet, falls back to system fonts offline).
- The contact form opens a pre-filled email. Wire it to a form service such as Formspree before launch.
- The animation lives at assets/techbunny-scale.gif. For best performance later, swap it for an MP4 or a compressed video.
