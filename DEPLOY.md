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

## GoDaddy redirect to GitHub Pages

If your domain is registered at GoDaddy and you want it to point to this GitHub Pages site (the repository already contains a `CNAME` file with `techbunny.ai`):

1. In the repository: keep the `CNAME` file at the repo root containing `techbunny.ai` (already present).
2. In GoDaddy DNS settings for `techbunny.ai` (apex/root): add four A records pointing the root (`@`) to GitHub Pages IPs:

	- 185.199.108.153
	- 185.199.109.153
	- 185.199.110.153
	- 185.199.111.153

3. For `www.techbunny.ai` create a CNAME record that points to your GitHub Pages domain (typically `TechbunnyLLC.github.io`).
4. Remove any GoDaddy forwarding rules for the domain (Page Forwarding interferes with Pages DNS).
5. Wait for DNS to propagate (can take up to 48 hours, usually faster). Then enable HTTPS in your repository Settings → Pages; GitHub will provision a certificate.

Notes:
- Use A records for the apex/root domain and a CNAME for `www` — you cannot set a CNAME at the apex.
- If GoDaddy supports ALIAS/ANAME you can use that for the apex instead of A records.
- If you want, I can add the exact `CNAME` target (e.g., `TechbunnyLLC.github.io`) — confirm the GitHub Pages publishing domain first.
