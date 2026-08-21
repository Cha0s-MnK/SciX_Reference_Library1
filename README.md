# Reference Library 1

Private PDF storage for the Reference Library web interface.

The repository keeps one small catalog at the root and stores each paper with
its sidecar metadata under `papers/<stable-paper-id>/`:

```text
catalog.json
papers/
  <stable-paper-id>/
    <paper-filename>.pdf
    metadata.json
```

`catalog.json` is the index used by the web interface. The PDF is served only
through the authenticated application; do not publish this repository or put
tokens in it.

The initial import was generated from the uploaded `Supermassive Black Holes
(SMBHs).zip` archive. Titles, authors, years, and tags are editable in the
interface after import.
