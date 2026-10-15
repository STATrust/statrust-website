# STATrust.ai — Launch Website

A responsive, dependency-light static landing page for STATrust. Inspired by the polished clinical-AI layout conventions of HopeAI, but with original visual design and copy focused on trustworthy agentic AI.

## Preview locally

```bash
python3 -m http.server 8000
```

Open http://localhost:8000.

## Recommended deployment: GitHub → Cloudflare Pages

1. Create or open the `statrust-website` repository.
2. Upload the contents of this folder at the repository root (including `index.html`, not just this README).
3. In Cloudflare Workers & Pages, connect the GitHub repository to a Pages project.
4. Select no framework / static HTML. Build command: `exit 0`. Build output directory: `.`.
5. Set the production branch to `main`; deploy.
6. In Pages > Custom domains, add `statrust.ai`. Follow Cloudflare's displayed DNS verification instructions.
7. Add `www.statrust.ai` as a second hostname and configure a redirect to the preferred hostname if desired.

If your Cloudflare Pages project already uses Git integration, update the repository rather than creating a new Direct Upload project.

## Before publishing

- `mailto:contact@statrust.ai` is **a placeholder**. Replace with a working address until you configure mail for the domain.
- The site presents SkillForge-BE and the certification layer as **in development / research**; it does not assert operational certification.
- The website does not run Python, R or an LLM. Host the application separately (for example, at `be.statrust.ai`).
- Review wording, affiliation, research references, product launch status, IP/branding and privacy terms with the team.
- No user-upload or API-key form has been added to this static site.

## Files

- `index.html` — content and structure
- `styles.css` — responsive design
- `script.js` — mobile navigation
- `favicon.svg` — logo mark
