# SciX Reference Library 1

Public, read-only data for a fast SciX-style reference catalogue.

The repository keeps one small index at the root and stores each refreshed PDF
with its sidecar metadata under `papers/<stable-paper-id>/`:

```text
catalog.json
papers/
  <stable-paper-id>/
    <paper-filename>.pdf
    metadata.json
```

`catalog.json` is the index consumed by the catalogue web application. Each
record includes the paper identifiers, source URL, source type, access note,
file size, and the GitHub path used to load the PDF.

The PDFs in this revision were downloaded afresh from openly accessible
publisher or preprint sources identified through SciX. Publisher PDFs are
used where SciX exposes an open route; otherwise the record uses an open
preprint PDF. Paywalled publisher copies are not bypassed or redistributed.

This repository contains no access tokens, PDF viewer state, or annotation
sidecars. The web application is intentionally read-only: it provides catalogue
search and filters and opens the stored PDFs as external GitHub links.
