# Crawl, index and licensing hygiene

By Ivan Stegic, 2026-09-23

Two questions that turn out to be one: what may a machine do with this content, and can it get to the content in the first place without drowning in duplicate URLs.

## What it measures

Licensing posture — whether machine-readable terms exist and travel with the content into feeds and schema. And index hygiene — whether missing pages return a real 404, whether redirects resolve in one hop, whether the crawlable URL space is finite, whether sitemap timestamps are a freshness signal or deploy noise, and whether the sitemap is structured so that crawl coverage can be diagnosed at all.

## How this site handles it

The sitemap here is an index pointing at a typed child rather than one flat list. Missing pages return a real 404 rather than a thin page with a 200. No URL on the site carries a query string, so the parameter space is not merely controlled but empty. Each page's timestamp comes from when its content last changed, never from the build, which is the distinction the freshness test exists to catch. The licence itself is published as an RSL 1.0 document at /license.xml, referenced from robots.txt and from the head of every page: all uses permitted, attribution requested, CC BY-SA 4.0 as the terms.

## Weight

12 of the hundred points, across 10 tests. The full definitions are in the open
standard at https://readinessindex.io/open-standard
