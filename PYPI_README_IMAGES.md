# PyPI README images

PyPI renders the `acp-ai` package README but **does not host images**. Browsers load each `![...](https://...)` URL directly.

Images are hosted in this **public** repo:

```text
https://raw.githubusercontent.com/raja-datascientist/acp-docs/main/images/<file>
```

## Verify before PyPI upload

From the ACP monorepo:

```bash
cd sdk/python
python3 scripts/verify_pypi_readme_images.py
```

All image URLs in `sdk/python/README.md` should return HTTP 200 anonymously.
