# Custom part shadows

Shadow (connectivity) files for our own parts — the ones kept in
`ldraw-parts/custom_parts/`. Same layout as `parts/` (subparts in `custom_parts/s/`),
same file names as the part they describe.

They publish to the CDN alongside `parts/` and `p/` and are looked up by part id, so
nothing that reads connectivity needs to know which folder a file is in. A file here
whose name also exists in `parts/` or `p/` fails the publish (`scripts/build-library.mjs`).

The connectivity editor saves shadows for custom parts here automatically.
