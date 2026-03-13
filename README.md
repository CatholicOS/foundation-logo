# Catholic Digital Commons Foundation — Logo Symbolism

This repository contains the **official description of the symbolism and conceptual imagery of the Catholic Digital Commons Foundation logo**, maintained as a version-controlled
public record.

The authoritative text is located in [`CDCF Logo Symbolism.md`](./CDCF%20Logo%20Symbolism.md).

---

## Why the logo symbolism lives in Git

The Catholic Digital Commons Foundation exists to steward shared digital goods with clarity, accountability, and continuity. Maintaining the official description of the
Foundation's logo in a Git repository directly serves that mission.

Version control provides:

### 1. Transparency

All changes to the logo's symbolic description are publicly visible, attributable, and reviewable. There are no silent edits and no ambiguity about how the Foundation articulates
the meaning of its visual identity.

### 2. Historical integrity

Git preserves the complete revision history of the document, allowing the Foundation and external stakeholders to trace how the logo's interpretation has been expressed over time.

### 3. Accountability

Each modification is associated with a concrete proposal, discussion, and approval record, reinforcing responsible governance.

### 4. Durability

Plain-text Markdown ensures the description remains readable and usable decades into the future, independent of proprietary formats or platforms.

### 5. Alignment with the Foundation's mission

As a foundation committed to open, shared digital infrastructure for the Church, it is fitting that its own identity documents are maintained using open, inspectable tools.

---

## Purpose of this document

A logo is more than a graphic: it is a condensed expression of an organization's identity, mission, and values. The Catholic Digital Commons Foundation's logo carries layered
theological and institutional meaning that deserves careful articulation.

This document serves several purposes:

- **Institutional memory** — It records the intended symbolism so that the meaning is preserved as the Foundation grows and leadership transitions occur.
- **Trademark protection** — A clear description of the logo's conceptual content supports trademark registration and defense.
- **Communication** — It provides an authoritative reference for anyone seeking to understand or present the Foundation's visual identity.

---

## Authority of the text

The content of [`CDCF Logo Symbolism.md`](./CDCF%20Logo%20Symbolism.md) constitutes the **official symbolic description** of the Catholic Digital Commons Foundation logo, subject
to adoption and revision according to the procedures defined in the Foundation's governance documents.

The Git history records _how_ the text has evolved; the Foundation's governance procedures define _when_ changes take effect.

---

## Local development

After cloning the repository, install the Node dev-dependencies:

```sh
npm install
```

### Available build scripts

| Command                         | Output                                                                                        |
| ------------------------------- | --------------------------------------------------------------------------------------------- |
| `npm run build:html`            | HTML fragment in `dist/logo-symbolism.html`                                                   |
| `npm run build:html:standalone` | Self-contained HTML (with embedded fonts and styles) in `dist/logo-symbolism-standalone.html` |
| `npm run build:pdf`             | PDF in `dist/logo-symbolism.pdf` (built from the standalone HTML)                             |

This requires [Pandoc](https://pandoc.org/) as a **system dependency** (not installed via npm). Install it first — for example `sudo apt install pandoc` on Debian/Ubuntu,
`brew install pandoc` on macOS, or see the [Pandoc installation docs](https://pandoc.org/installing.html).

---

## Releases

Each version of the logo symbolism is published as a [GitHub Release](../../releases) with a standalone HTML file, a PDF, and a press kit zip.

Releases are created automatically by the CI workflow when a version tag is pushed. **Do not create a GitHub Release manually** — create only the tag, and let the workflow do the
rest.

To publish a new release:

```sh
git tag v1.x
git push origin v1.x
```

The workflow will build the artifacts and create the release. If you do create a release manually (e.g. through the GitHub UI), the workflow will detect the existing release and
upload the built assets to it rather than failing.

---

## License and reuse

This repository contains identity documents of the Catholic Digital Commons Foundation. Reuse or adaptation for other organizations should respect applicable legal and canonical
requirements.
