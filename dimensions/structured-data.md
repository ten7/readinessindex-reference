# Structured data and the entity graph

By Ivan Stegic, 2026-09-22

An Organization block and some FAQ markup is commodity work. A linked graph, anchored to records somebody else controls and validated so it cannot rot, is not.

## What it measures

Whether schema follows the content or was typed into a template. Whether a page declares where it sits in the information architecture. Whether the site models the things it actually contains, using the types its declared vertical expects. And, since version 11.0, whether the markup is simply valid: every block parsing, every node carrying the properties its type needs, dates in ISO 8601, URLs absolute, prices with a currency.

## How this site handles it

The declared vertical here is research, and the site genuinely holds all three types that vertical expects: the check registry as a Dataset, the published data as a DataCatalog, and the standard itself as a ScholarlyArticle. Every page below the homepage carries a breadcrumb trail that matches its URL. Value objects such as postal addresses and breadcrumb lists deliberately carry no identifier, because they have no identity and nothing should ever point at them.

## Weight

15 of the hundred points, across 8 tests. The full definitions are in the open
standard at https://readinessindex.io/open-standard
