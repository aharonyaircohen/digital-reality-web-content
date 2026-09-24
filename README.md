# Digital Reality Web Content

Public dataset for Digital Reality websites. This repository currently contains the imported WordPress archive and its related metadata and media. It is a website content store; it is not the primary workspace for Yair's new original writing.

## Current structure

- `posts/`, `pages/`, and `courses/` — imported public WordPress records, in `<wordpress-id>-<slug>` folders.
- `learndash/courses/` — imported LearnDash hierarchy, including course material and associated legacy/shared items.
- `learndash/media/` — locally stored LearnDash media.
- `index.json`, `pages-index.json`, and `courses-index.json` — catalogues. Post
  entries with a featured image include its repository-relative
  `featured_media_path` so public sites can render thumbnails without a metadata
  API request for every post.
- `archive-report.json` and `export-report.json` — export and archive reports.

A standard WordPress record may contain `content.md` (readable Markdown), `source.html` (exported HTML), `metadata.json` (source and publication metadata), and `media/` (local images and other non-video files). External videos remain links. LearnDash records preserve hierarchy and metadata within `learndash/courses/`.

The imported archive includes posts, pages, a public course, and LearnDash course material. The repository root currently has no `source-exports/` directory; do not rely on that older documentation path for an original WXR file.

## Relationship to writing and public sites

| Repository | Role |
| --- | --- |
| [digital-reality-source](https://github.com/aharonyaircohen/digital-reality-source) | Private home for Yair's original writing, ideas, research, book manuscript, and authored content. |
| This repository | Public website records and imported content. It can hold published or prepared records, but presence here does not grant publication status. |
| [digital-reality-me-web](https://github.com/aharonyaircohen/digital-reality-me-web) | Public profile and article site. The visitor's browser reads this repository's `index.json` and loads only published posts from the API. |
| [digital-reality-web-book](https://github.com/aharonyaircohen/digital-reality-web-book) | Public web reader and its chapter publication copy. |

The website source and public sites are separate repositories. Compare the relevant record, status, and published copy when updating; no automatic sync is implied.

## Profile page assets

`pages/3988-yac/media/` also holds the optimized profile-site images and its
sharing artwork. These variants were previously stored in `digital-reality-me-web`;
they now live here as the only maintained copies. The profile site links directly
to these public files. They preserve the current site images, including the
dehydration variant without a text overlay. The imported `metadata.json` still
describes original WordPress media; its references do not guarantee every original
file was included in the export.
