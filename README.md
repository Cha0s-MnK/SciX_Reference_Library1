# SciX Reference Library

A fast, read-only paper catalogue backed by the public SciX libraries.

## Contents

- 69 paper records from 14 SciX libraries.
- One tag per paper: the exact SciX library name.
- One PDF per record under `papers/`, downloaded from the SciX full-text source selected for that record.
- `catalog.json` contains the searchable metadata and source links.

Publisher PDF sources are used where the SciX publisher route returned a valid PDF in the build environment. Where a publisher route returned an access or bot-check page, the record uses SciX's open Preprint PDF source instead. The catalogue keeps the publisher link in `publisherSourceUrl` when SciX exposed one.

This repository contains no editing, annotation, or PDF-viewer state.
