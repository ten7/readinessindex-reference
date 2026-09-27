# Alternate representations

By Ivan Stegic, 2026-09-26

Read this before you sell it: evidence that these files are consumed by the major models remains thin. They are here because they are cheap, they force good content hygiene, and being early costs nothing.

## What it measures

Whether every canonical page has a Markdown companion that matches the page body without the navigation chrome. Whether that companion is advertised in the head so it can be found. Whether the canonical URL itself will serve Markdown to a client that asks for it, with the cache headers that make doing so safe. And whether these generated files are served from an edge cache rather than regenerated on every request.

## How this site handles it

Every page here has a Markdown twin with the nav, the breadcrumb and the footer stripped out, advertised from the head and served with the right content type. They are edge-cached. Content negotiation on the Accept header is the one test in this dimension the site does not pass: it requires a rewrite at the edge, and this site is served directly from GitHub Pages with no proxy in front of it. Getting that wrong would be worse than not doing it, so it is left undone and said out loud.

## Weight

8 of the hundred points, across 4 tests. The full definitions are in the open
standard at https://readinessindex.io/open-standard
