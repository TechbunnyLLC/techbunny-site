# TechBunny.ai — Project Brief

Context handoff for continuing this project (in Cowork, with Greg, or a fresh session).

## Positioning (do not drift from this)
TechBunny is a senior, US-led product and software engineering studio. We deliver the full solution: scope, architecture, and shipped product. We own the outcome.
- Not a staffing desk. Not a way to "hire offshore engineers."
- Delivery method (global team, CoderPush partnership) stays QUIET. Never name CoderPush on the site. Never frame TechBunny as a reseller or offshore-hiring service.
- Cost efficiency is a late closer, never the headline.
- Tagline: "Bunnies know how to scale." Brand line: "Silicon Valley architecture. Bunny-fast execution."

## Voice and style rules
Plain, direct prose. Active voice. No filler, no buzzwords. No em dashes (use commas, periods, colons). Should read like a person wrote it, not an LLM. Make claims concrete and citable.

## Brand
- Colors: aqua #B6FCFC (anchor), ink #0B1722 (text), amber #FF8A2B (accent, pulled from the logo goggles).
- Logo: line-art tech-bunny (header/footer mark). Cyber-bunny render is retired.
- Hero centerpiece: scaling-bunnies GIF (assets/techbunny-scale.gif).

## Team bios (facts and flags)
- Greg Argyle, CEO/Lead Architech, founded rSportz.com in 2006, CTO through 2021. Silicon Valley original who helped build the Netscape browser, created the first customizable enterprise browser for AOL/Time Warner, engineer for SCO Unix/Red Hat Lynix (Todd confirmed via Greg's LinkedIn; not independently verified by search).
- Todd Johnson, CRO. Co-founded and scaled rSportz.com; led the acquisition and $13M+ funding; grew to 3M+ athletes in 100+ countries; 2020 exit. Inc. 500 winner, built the 89th fastest-growing US company (this traces to SKM Media Group, 2013, 3,751% growth, not rSportz; framed as his personal achievement).
- Partners trained at Yale and Harvard: rests on Todd's word (not independently verified).
- Partnership: Todd and Greg since 2006.

## Clients (current, paying) — Work section, each logo links out
1. Coin Theaters (cointheaters.com) — flagship, full website and platform built by TechBunny. Crowdfunding + streaming + social.
2. photo-op.ai — AI media and UGC licensing platform.
3. Entertainment Octopus (entertainmentoctopus.com) — prop and film rental company platform and apps.
4. AromaTech (aromatech.com) — product platform and mobile apps.
5. Hireons (hireons.com) — AI hiring and interview platform.
EO and AromaTech are paying clients per Todd.

## Site sections (built)
Hero (GIF + positioning + proof chips), stat band, problem/answer, What We Build, AI in Production (pilot-to-production, agentic, data, cloud, plus a pre-ship discipline framework), How We Work, Work (5 clients), Team, About, FAQ, Working With Us (communication advantage + engagement CTAs), manifesto band, Contact. CTAs throughout.

## Tech
Site: hand-coded static HTML + CSS + vanilla JS. Host on AWS S3 + CloudFront (see DEPLOY.md). Fonts from Google Fonts.
Showcased build capabilities: AWS, AWS IoT, Flutter, React Native, Stripe, Shopify, blockchain/crypto, AI/ML.

## Pending before launch
1. Wire the contact form to a service (e.g. Formspree). It currently opens a pre-filled email.
2. Add JSON-LD SEO schema (Organization, Service, FAQPage).
3. Swap the embedded/standalone GIF for an MP4 or compressed video for performance.
4. Validate the SEO keyword list before committing copy to it.
5. Optional: have a designer rebuild the line-art logo as clean vector source.

## Assets in this folder
index.html, DEPLOY.md, assets/ (logo-mark.png, techbunny-scale.gif, photo-op.png, eo.jpg, aromatech.jpg, hireons.png, coin.jpg).
