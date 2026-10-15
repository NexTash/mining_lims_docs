# NexTash product documentation

User documentation for NexTash products, published with MkDocs Material at
https://nextash.github.io/mining_lims_docs/

| Product | Folder |
| --- | --- |
| Mining LIMS | `docs/mining-lims/` |

## Editing

Pages are plain Markdown under `docs/`. Edit on GitHub or locally:

```bash
pip install mkdocs-material
mkdocs serve        # preview at http://127.0.0.1:8000
```

Every push to `main` publishes the site through GitHub Pages (`.github/workflows/deploy.yml`).
Add a product by creating a folder under `docs/` and adding its pages to `nav` in `mkdocs.yml`.
