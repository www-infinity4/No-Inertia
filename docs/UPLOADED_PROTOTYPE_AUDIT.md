# Uploaded No Inertia Prototype Audit

Two uploaded HTML prototypes were reviewed for integration.

## `no-inertia-8.html`

- 221 lines
- generic light website template
- placeholder headings such as “Section Heading,” “Our Features,” and “Our Impact”
- remote Google fonts
- remote Unsplash images
- no project-specific calculations or simulator logic
- no localStorage, fetch, canvas, or application state

SHA-256 prefix: `d3d2ab2c7740e800`

## `no-inertia-.html`

- 761 lines
- larger generic business/portfolio template
- remote Google fonts, Unsplash images, and avatar services
- two forms and an iframe
- placeholder branding and generic calls to action
- no No-Inertia scientific engine or measured-data model

SHA-256 prefix: `6d311af5881cb855`

## Decision

Neither uploaded file should replace the repository’s main page. They are visual mockups, not functioning No-Inertia research applications.

Useful pieces to retain:

- responsive section spacing;
- sticky navigation pattern;
- gallery and statistics layouts;
- contact/feedback layout;
- phone-width container rules.

Pieces to reject or replace:

- generic “Logo” and stock copy;
- remote stock photography;
- remote avatar service;
- inline mouseover handlers;
- iframe content without an explicit allowlist;
- forms without a real privacy and submission backend;
- desktop-first navigation that becomes cramped on mobile.

## Rebuild target

The working No-Inertia application should contain:

1. Readable project definition and claim ledger.
2. Inertia/reference-frame visualizer.
3. Acceleration, momentum, and energy comparison graphs.
4. User-defined project-model layer kept separate from established mechanics.
5. Finite Curvature Limit integration for determining where ideal motion models stop matching measured data.
6. Sensor import for accelerometer and gyroscope logs.
7. Mobile-first controls at least 44 px high.
8. Offline operation and JSON export.
9. No third-party tracking or remote stock assets.
10. A clear statement that “no inertia” is a project hypothesis or simulation mode, not a proven reactionless propulsion mechanism.

## Proposed structure

```text
/
├── index.html
├── app.css
├── app.js
├── data/claims.json
├── docs/SCIENTIFIC_MODEL.md
├── docs/EXPERIMENT_PROTOCOL.md
├── prototypes/no-inertia-8-original.html
└── prototypes/no-inertia-large-original.html
```

The original files should be preserved under `prototypes/` once binary/file transfer is available, but they should not be deployed as the primary product.