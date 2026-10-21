# Affiliate Lab

Developed by SEO Girl - Ami. A standalone affiliate marketing portfolio app with campaign planning, an AI content studio, an opportunity finder and revenue scenarios.

## Try the app
Open index.html in a browser. The prepared demos work without a model call. Internet access is required to generate fresh content with Gemini.

## GitHub and Vercel
Suggested repository name: affiliate-lab

1. Upload index.html, vercel.json and README.md to the repository root.
2. Import the repository into Vercel.
3. Choose the Other framework preset. No install or build command is required; serve the repository root.
4. Deploy and test AI generation on the live URL.

## Gemini connection
The app uses the existing server-side proxy at:
https://gemini-proxy-boldstudio.vercel.app/api/gemini

Model: gemini-3.8-flash

Keep GEMINI_API_KEY in the proxy project's Vercel environment variables. This frontend project does not need its own API key while using that proxy. Never put keys in index.html or GitHub. Generation depends on the proxy's availability, access configuration, CORS and API quota. This package does not alter the proxy's access controls or rate limits.

## Included features
- Campaign planning and sample offer comparisons
- Prepared travel, reading and creator-software demos
- Gemini content generation, editing, review notes and exports
- Opportunity Finder with search and affiliate CSV import, sample data, transparent ranking and AI recommendations
- Revenue scenario calculator

## Data and limitations
CSV reports are processed locally. Generating content or recommendations sends the relevant brief, source notes and selected opportunity to Gemini through the proxy. Sample offers, products and performance data are fictional. Opportunity scores and revenue calculations use explicit assumptions, not predictive AI. The app does not crawl pages, verify merchant terms, connect to affiliate networks or publish content. Review claims and links before use.

Saved drafts use browser storage. Reports are not saved. Export drafts and reports to keep backups. No dependency installation or external frontend library is needed.

## Verification
Automated checks covered CSV handling, opportunity ranking, missing-data handling, AI response/error handling and the studio handoff. The proxy returned a successful real Gemini response during development. Browser visual QA and Vercel deployment remain unverified.
