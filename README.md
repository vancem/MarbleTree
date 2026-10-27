# Laser-Cut Marble Tree

**Read it online: <https://vancem.github.io/MarbleTree/>**

How to laser-cut and assemble a wooden marble tree toy, by [Vance Morrison](https://vancem.github.io/VancePMorrison/).
The design files (SVG) are in `docs/design/` and open in a browser.
Two short films of the finished toy are in `docs/videos/`.

## How the site is built

The book is Markdown in `docs/`. The chapter order is the `nav` list in `mkdocs.yml`.
[MkDocs Material](https://squidfunk.github.io/mkdocs-material/) builds the site, and the
`Deploy site` GitHub Action publishes it to GitHub Pages on every push to `main`.

To preview locally:

```
pip install -r requirements.txt
mkdocs serve        # preview at http://127.0.0.1:8000/MarbleTree/
```

The public address works after the repository is on GitHub and Pages is set to GitHub Actions.
