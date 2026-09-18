---
# The paper's title, exactly as published (or as submitted, for a preprint).
title: "{{ replace .Name "-" " " | title }}"

# Publication date (YYYY-MM-DD). Controls the order papers are listed in
# (newest first). For a preprint, use the date it was first made public.
date: {{ .Date }}
draft: false

# List every author, in author order.
# - A DiNum-GEO team member: use the filename (without ".yaml") of their
#   entry in data/authors/ -- "milos", "ksenija", or "me" -- and it will
#   automatically link to their profile and show their photo below.
# - Anyone else: just write their name as plain text.
authors:
  - milos
  - "External Co-Author Name"

# Exactly one of: paper-conference, article-journal, article (used for
# preprints), report, book, chapter, thesis, patent
publication_types: ["article-journal"]

# Where it was/will be published. Delete this whole block if there is no
# venue yet (e.g. a preprint not yet submitted anywhere).
publication:
  name: "Journal or conference name"
  volume: ""
  issue: ""
  pages: ""
  publisher: ""

# 2-4 sentence summary, shown in a box on the paper's own page.
abstract: >-
  Write a short abstract here.

# Optional status flags -- delete either line if not applicable.
peer_reviewed: false
open_access: false

tags: []
---

<!--
  Add a DOI and/or PDF link below as plain Markdown -- do NOT use a
  "links:" or "hugoblox.ids:" front matter field for this: a bug in the
  current theme build crashes the whole site if either is used on a
  content page. This plain-Markdown form works and looks the same.

  For a PDF, drop the file next to this index.md (e.g. paper.pdf) and
  link to its filename instead of a URL.
-->

**DOI:** [10.xxxx/xxxxx](https://doi.org/10.xxxx/xxxxx)

Add any longer notes here (optional) -- this text appears below the
abstract box on the paper's own page. Delete this line if the abstract
is enough on its own.
