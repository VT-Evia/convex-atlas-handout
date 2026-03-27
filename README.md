# ConVEx Atlas Handout

Companion handout for **Navigating ContentOps, DITA, Markdown, and AI: A ConVEx Atlas**  
ConVEx Pittsburgh · Monday, April 13, 2026 · 10:30–11:15 AM

**Carlos Evia** · Virginia Tech  
**Rebekka Andersen** · University of California Davis

---

## Live Handout

👉 **[vt-evia.github.io/convex-atlas-handout](https://vt-evia.github.io/convex-atlas-handout)**

---

## Contributing

This handout is maintained as an open, versioned document. If you find an error, want to suggest a revision, or have a resource to add:

1. Open an [issue](../../issues)
2. Or fork the repo, make your changes, and open a pull request

Every push to `main` automatically deploys to GitHub Pages via GitHub Actions. Pull requests trigger a build-only validation step — no deploy until merged.

---

## Local Development

```bash
pip install mkdocs-material
mkdocs serve
```

Then visit `http://localhost:8000`.

---

## Structure

```
docs/
├── index.md        # Main handout (session overview, core claims, key terms)
├── concepts.md     # The Atlas: Key Concepts (five territories)
├── paths.md        # Suggested Paths (four practitioner routes)
└── resources.md    # References, tools, further reading
mkdocs.yml          # Site configuration
.github/workflows/
└── deploy.yml      # CI/CD pipeline
```
