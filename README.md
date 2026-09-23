# Digital Reality Web Content

Private dataset for Digital Reality websites. This repository currently contains the imported WordPress archive and its related metadata and media. It is a website content store; it is not the primary workspace for Yair's new original writing.

## Current structure

- `posts/`, `pages/`, and `courses/` — imported public WordPress records, in `<wordpress-id>-<slug>` folders.
- `learndash/courses/` — imported LearnDash hierarchy, including course material and associated legacy/shared items.
- `learndash/media/` — locally stored LearnDash media.
- `index.json`, `pages-index.json`, and `courses-index.json` — catalogues.
- `archive-report.json` and `export-report.json` — export and archive reports.

A standard WordPress record may contain `content.md` (readable Markdown), `source.html` (exported HTML), `metadata.json` (source and publication metadata), and `media/` (local images and other non-video files). External videos remain links. LearnDash records preserve hierarchy and metadata within `learndash/courses/`.

The imported archive includes posts, pages, a public course, and LearnDash course material. The repository root currently has no `source-exports/` directory; do not rely on that older documentation path for an original WXR file.

## Relationship to writing and public sites

| Repository | Role |
| --- | --- |
| [digital-reality-source](https://github.com/aharonyaircohen/digital-reality-source) | Private home for Yair's original writing, ideas, research, book manuscript, and authored content. |
| This repository | Private website records and imported content. It can hold published or prepared records, but presence here does not grant publication status. |
| [digital-reality-me-web](https://github.com/aharonyaircohen/digital-reality-me-web) | Public static profile and article site. Its checked-in post pages are refreshed from records with `status: "publish"` only. |
| [digital-reality-web-book](https://github.com/aharonyaircohen/digital-reality-web-book) | Public web reader and its chapter publication copy. |

The website source and public sites are separate repositories. Compare the relevant record, status, and published copy when updating; no automatic sync is implied.
