# Spontaneous Prose

All-English podcast. Public RSS on GitHub Pages; 小宇宙 binds this feed.

- Site: https://joycenotebook.github.io/spontaneous-prose/
- RSS: https://joycenotebook.github.io/spontaneous-prose/feed.xml
- Sister show (do not mix feeds): [发声 Taste, Out loud](https://joycenotebook.github.io/joyce-podcast/)

## Publish one episode

1. Put the mp3 in `audio/ep-XXX.mp3` (128 kbps is enough for speech; keep files under ~40 MB).
2. Put Show Notes HTML in `shownotes/ep-XXX.html`.
3. Append the episode in `episodes.json` (`id`, `title`, `file`, `duration_sec`, `size_bytes`, `desc`, `pub_date`, `listed`).
4. Run `python3 scripts/rss_gen.py`.
5. Commit and push `main`. GitHub Pages updates `feed.xml`; 小宇宙 usually picks it up in 1–24 hours.

Do not point 小宇宙 at the 发声 feed. Do not reuse 发声 episode ids, audio URLs, or guids.

Replace `cover.jpg` before the first public episode if this placeholder is not the final art.
