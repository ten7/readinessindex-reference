# Authorship, provenance, freshness

By Ivan Stegic, 2026-09-24

A byline string asserts nothing a machine can check. A resolvable entity with credentials does, and so does a date that only moves when the content moves.

## What it measures

Whether authors resolve to real, credentialed entities rather than names. Whether substantive pages are signed, and whether the author property is a reference to an identifier rather than a repeated string. Whether published and modified dates are internally consistent and stable across a deploy that changed nothing. On sites that warrant them, whether expert review and primary-source citations reach the markup.

## How this site handles it

Every page here is signed, visibly and in the schema, and the author property is a reference to one Person node rather than a name repeated ten times. That person carries a job title, an affiliation, subjects they work in, and an ORCID — an identifier somebody else had to grant. Dates come from the content, not the build, and the sitemap agrees with the page.

## Weight

12 of the hundred points, across 6 tests. The full definitions are in the open
standard at https://readinessindex.io/open-standard
