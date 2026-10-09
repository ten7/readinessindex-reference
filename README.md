# readinessindex-reference

The reference implementation of the [Readiness Index](https://readinessindex.io/open-standard),
version **11.0** (effective 24 September 2026).

Live at **https://reference.readinessindex.io**

A standard nobody has satisfied is a hypothesis. This repository is the attempt to
satisfy one in public, with the working shown: a hand-written, no-JavaScript static
site, served from GitHub Pages, built to score as close to 100 as the Index allows.

## What is here

```
index.html                     the homepage
contact.html                   served at /contact
dimensions.html                served at /dimensions
dimensions/*.html              one page per dimension, seven of them
*.md                           a Markdown companion beside every page  (AIR-7.1)
robots.txt                     crawler permissions, Content Signals, AI policy prose
llms.txt                       llmstxt.org index of the site
license.xml                    the RSL 1.0 licence, referenced from robots.txt  (AIR-4.1)
sitemap.xml                    a sitemap index
sitemap-pages.xml              top-level pages
sitemap-dimensions.xml         the dimension pages
sitemap-images.xml             the diagram, with the image namespace
dimensions.svg                 the seven dimensions and their weights
style.css                      one stylesheet
.nojekyll                      GitHub Pages serves these files as-is
```

Ten pages and the machine-readable files that describe them. No framework, no
content management system, and nothing on the page that a browser has to execute,
because none of those are what the Index measures.

## Design rules

**No JavaScript.** The heaviest single test in the Index — six of the hundred points —
measures how much of a page survives without it. A site with none passes by
construction.

**No forms, no search, no query strings.** Not austerity for its own sake: the Index
scores a site on the markup it needs, so a site that has no search cannot fail the
search test. Twelve of the fifty-one tests pass this way, worth twenty-one points, and
the homepage says so out loud rather than banking it quietly.

**One linked entity graph.** Three canonical `@id`s — Organization, WebSite, Person —
defined once and referenced everywhere. Value objects such as `PostalAddress` and
`BreadcrumbList` deliberately carry no `@id`, because they have no identity and nothing
should point at them.

**Every claim is checkable.** Every fact in the markup is a real fact about TEN7, and
every `sameAs` target resolves. A reference implementation that cheated would be worth
less than no reference implementation at all.

## Verifying it

Scan it with any implementation of the standard, including your own. The specification
is published under CC BY-SA 4.0 and is complete enough to build a scanner from:

- The standard: https://readinessindex.io/open-standard
- The check registry: the fifty-one scored tests, their weights and their band rules

If you find something here that does not match what the standard requires, that is a
bug worth reporting — open an issue, or write to hello@readinessindex.io.

## What this does not claim

It does not claim to be a good website in any other sense. The Index measures whether
machines can find, read, trust and use a site. It does not measure design, prose,
usefulness or accessibility conformance, and neither does this repository.

It is also not yet at 100. Some of the remaining points depend on response headers that
GitHub Pages cannot set, and some depend on inputs a scan has to be given rather than
read. Both are tracked, and the score is published with its arithmetic rather than
rounded into a claim.

## Licence

Content and markup: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
Published by [TEN7](https://ten7.com/).
