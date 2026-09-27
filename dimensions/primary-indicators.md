# Primary Indicators

By Ivan Stegic, 2026-09-19

Thirty of the hundred points sit here, more than any other dimension. Not because reachability matters more than everything else, but because this is the sum of the strongest test pulled from each of the others — the things a single page can answer.

## What it measures

Whether a crawler is allowed in at all, and whether the edge honours that. Whether the site states a machine-readable position on search, AI input and AI training. Whether one page is enough to work out who publishes it, what it is called, and which organization it belongs to. Two of the thirteen are gates: if robots.txt turns answer engines away, or the CDN quietly returns 403 to them, none of the rest is reaching anybody.

## How this site handles it

The robots.txt here disallows nothing and names all ten agents as welcome, with the position written out in prose above the machine-readable line so a person reading the file understands it too. Every page emits an absolute self-referencing canonical, carries exactly one h1, and never skips a heading level. Three canonical identifiers — the organization, the site and the author — are defined once and referenced everywhere rather than restated.

## Weight

30 of the hundred points, across 13 tests. The full definitions are in the open
standard at https://readinessindex.io/open-standard
