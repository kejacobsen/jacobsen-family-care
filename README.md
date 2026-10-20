# Jacobsen Family Care

Public website for **Jacobsen Family Care**, a caregiver coordination text service by Katie Jacobsen.

**Live site:** https://kejacobsen.github.io/jacobsen-family-care/

| Page | URL |
| --- | --- |
| Home (how to join) | https://kejacobsen.github.io/jacobsen-family-care/ |
| Privacy Policy | https://kejacobsen.github.io/jacobsen-family-care/privacy.html |
| Terms & Conditions | https://kejacobsen.github.io/jacobsen-family-care/terms.html |

## How it's built

The site is written in Markdown and built with [Zensical](https://zensical.org). Pushing to `main` runs the GitHub Actions workflow in `.github/workflows/docs.yml`, which builds the site and publishes it to GitHub Pages.

```
docs/
├── index.md      # landing page and opt-in instructions
├── privacy.md    # Privacy Policy
└── terms.md      # Terms & Conditions
zensical.toml     # site settings and navigation
```

## Working on it locally

```
uv sync
uv run zensical serve
```

Then open http://localhost:8000. Edits to files in `docs/` reload automatically.

## Keeping things consistent

The phone number, opt-in keyword (JOIN), confirmation message, and disclosures on these pages must match what's registered with the messaging provider. If any of them change, update the site and the registration together, and bump the "Last updated" date on the Privacy Policy and Terms.
