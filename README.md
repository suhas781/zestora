# Zestora

Static marketing site for Zestora — honest, nutrient-dense snacks.

## Local preview

Open `index.html` in a browser, or from this folder run:

```bash
npx --yes serve .
```

Then visit the URL shown (usually http://localhost:3000).

## Deploy on GitHub Pages

1. In the repo on GitHub: **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **GitHub Actions** (not “Deploy from a branch”). Save if prompted.
3. Push to `main`, or open **Actions → Deploy static content to Pages → Run workflow**.

If this step is skipped, the workflow usually fails in a few seconds on **Setup Pages** (`configure-pages`) because GitHub Pages is not configured to accept Action deployments yet.

The live URL will be `https://suhas781.github.io/zestora/` after a successful run.

### If the workflow still fails

- **Settings → Actions → General → Workflow permissions**: use **Read and write permissions** (or keep defaults that allow the workflow’s `permissions:` block).
- Re-run the job from the **Actions** tab after changing Pages or token settings.
