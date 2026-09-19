# Content Library

Archive of WordPress posts from The Digital Reality.

## Structure

Each directory under `posts/` is named `<wordpress-id>-<slug>` and contains:

- `content.md` — readable Markdown content.
- `source.html` — original WordPress HTML with local media paths.
- `metadata.json` — source, publishing, taxonomy, SEO, media, and video-link metadata.
- `media/` — downloaded images and non-video files used by or attached to the post.

Videos are intentionally preserved as external links and are not downloaded.
`index.json` provides a machine-readable catalogue of all posts.
