# Content Library

Archive of public WordPress content from The Digital Reality.

## Structure

Each directory under `posts/`, `pages/`, and `courses/` is named `<wordpress-id>-<slug>` and contains:

- `content.md` — readable Markdown content.
- `source.html` — original WordPress HTML with local media paths.
- `metadata.json` — source, publishing, taxonomy, SEO, media, and video-link metadata.
- `media/` — downloaded images and non-video files used by or attached to the post.

Videos are intentionally preserved as external links and are not downloaded.
`index.json` provides a machine-readable catalogue of posts, pages, and the public `course` type.
`archive-report.json` records totals, media-download failures, and content types that require authenticated LearnDash access.

The archive contains 36 posts, 59 pages, 1 public course, and LearnDash content exported from WordPress: 14 courses, 93 lessons, 49 topics, 4 quizzes, 12 questions, and 4 certificates.

LearnDash metadata and hierarchy fields are preserved in each `metadata.json`. The original WXR export is kept under `source-exports/`. Local media is stored under `learndash/media/`; external videos remain as links.
