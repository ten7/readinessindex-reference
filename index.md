# A website built to score 100

By Ivan Stegic, 26 September 2026

This is the reference implementation of the Readiness Index, version 11.0. It is
hand-written, it ships no JavaScript, and it exists for one reason: to show that the
standard we publish is achievable rather than merely measurable. Anyone can read every
file it is made of, and anyone can re-run the scan that scores it.

## What this is

The Readiness Index asks one question: can machines find, read, trust and use this
website? It answers with a number between 0 and 100, computed from fifty-one tests
across seven dimensions, each with a published weight and a published rule for how it
is banded. The specification is free under CC BY-SA 4.0 and anyone may build their own
scanner from it.

A standard nobody has satisfied is a hypothesis. This site is the attempt to satisfy it
in public, with the working shown. It is two pages, a stylesheet, one diagram, and the
handful of machine-readable files the Index asks for. There is no framework, no build
tool and no content management system behind it, because none of those are what the
Index measures.

## The seven dimensions

Each dimension has its own page saying what it measures and what this site does about
it, including where it falls short: Primary Indicators, Rendering and extraction,
Structured data, Crawl and licensing hygiene, Authorship and freshness, Agent
interfaces and Alternate representations.

## How it scores

Thirty points come from the Primary Indicators — whether crawlers are allowed in,
whether the edge actually serves them, whether the site states a position on AI use,
and whether one page is enough to work out who publishes it. Fifteen come from
rendering: the single heaviest test in the Index asks how much of the page survives
without JavaScript, and a site with no JavaScript passes it by construction.

Another fifteen come from structured data, twelve from crawl and licensing hygiene,
twelve from authorship and freshness, and eight each from agent interfaces and
alternate representations. Every page here carries a Markdown companion, a
self-referencing canonical, a byline that resolves to a person, and one linked entity
graph rather than a pile of disconnected assertions.

## What passes by absence

Twelve of the fifty-one tests pass because this site does not contain the thing they
measure. There is no search, no form, no shop, no pagination and no API, so the tests
that score those things record that there is nothing to fix. That is the standard
working as designed — you cannot fail at markup you do not need — and it is worth
twenty-one of the hundred points.

We say so here rather than leave somebody to discover it. A reference implementation
that quietly banked a fifth of its score on being small would be making a weaker claim
than it appeared to, and the whole point of this site is that its claims can be checked.

## Who publishes it

TEN7 is a Minneapolis digital agency, founded on 16 April 2007, that designs, builds
and cares for Drupal websites for mission-driven organizations across the United
States. We publish the Readiness Index, we sell scans against it, and this site is
us being scored by our own instrument.

You can reach us at hello@readinessindex.io or on 612-868-7884.
