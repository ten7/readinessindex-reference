# Rendering and extraction

By Ivan Stegic, 2026-09-21

Most crawlers that feed answer engines do not execute JavaScript. This dimension asks a blunt question: how much of the page is actually in the server's response?

## What it measures

The gap between the raw HTTP response and the hydrated DOM, measured as a ratio and averaged across the sample. That single test carries six points, the heaviest in the Index. Around it sit tables with real header cells, alt text on content images, anchor identifiers stable enough to cite a passage rather than a page, and whether any key fact is trapped in an image or a PDF.

## How this site handles it

This site ships no JavaScript, so the raw response and the rendered page are the same document and the heaviest test passes by construction. Every heading below the h1 carries an identifier derived from its own text, so they survive a rebuild unchanged. There are no PDFs. The one diagram is an SVG whose numbers also appear in the prose beside it, because a fact that exists only inside a picture is a fact a parser cannot read.

## Weight

15 of the hundred points, across 6 tests. The full definitions are in the open
standard at https://readinessindex.io/open-standard
