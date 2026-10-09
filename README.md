# Facts & Context — GitHub Pages first

Stage 1: publish on GitHub Pages without a custom domain.
Upload these files to the repository root:

- index.html
- privacy.html
- terms.html
- styles.css
- README.md

Then:
Settings → Pages → Deploy from a branch → main → /(root)

Verify the default Pages URL works first:
https://YOUR_GITHUB_USERNAME.github.io/facts-context-site/

Stage 2: connect the custom domain facts.truthforum.us.

After the default site works:
1. GitHub Settings → Pages → Custom domain → facts.truthforum.us
2. In DNS for truthforum.us, create:
   CNAME  facts  →  YOUR_GITHUB_USERNAME.github.io
3. Wait for DNS/HTTPS provisioning.
4. Enable Enforce HTTPS when available.

Final URLs:
https://facts.truthforum.us/
https://facts.truthforum.us/privacy.html
https://facts.truthforum.us/terms.html
