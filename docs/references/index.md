---
layout: page
title: "References for participants"
---

## URNs

- *Iliad* text
    - Venetus B: `urn:cts:greekLit:tlg0012.tlg001.msB:`
    - Upsilon 1.1: `urn:cts:greekLit:tlg0012.tlg001.e3:`
- scholia text
    - Venetus B: `urn:cts:greekLit:tlg5026.msB.hmt:`
    - Upsilon 1.1: `urn:cts:greekLit:tlg5026.e3.hmt:`
- manuscript pages
    - Venetus B: `urn:cite2:hmt:msB.v1:`
    - Upsilon 1.1: `urn:cite2:hmt:e3pages.v1:`



Finding other URNs:

- [HMT URN search](https://interwing.nl/hmt/urn/) (from Leiden team member Mees Gelein)
- request URNs for new personal names, place names, etc using forms on the [`hmt-authlists` repository](https://github.com/homermultitext/hmt-authlists)

## HMT editors' guide

### Concise summary of XML usage

Our XML markup falls in 4 tiers:

1. *transcription level* (or, editorial status): unclear, gaps, etc
2. *tokenization level*: words, abbreviations, superlinear addtions, deletions, corrections, scribal multiforms, character strings
3. *editorial disambiguation level*: named entities
4. *discourse disambiguation*: quotations and citable references

At each level, the following TEI elements are allowed:


**Transcription level**

- `unclear`
- `gap`

**Tokenization level**


- `w`
- `num`
- `abbr/expan` choice
- `del` deleted by scribe (e.g., underdots)
- `add` text added (eg, above line)
- `orig/reg` choice: alternate reading offered (multiform)
- `sic/corr` choice: scribal correction

**Editorial disambiguation level**

Named entities with `@n` attribute with URN value:

- `persName`
- `placeName`
- `rs` with `@type` attribute


**Discourse level**


- `q` alone:  
    - quotation, work not extant
    - quoted example of language. Test: you would not  translate this when reading the text, e.g. explaining the declension of a noun by using another common Greek word as an example
- `cit` containing `q` and `ref`: quotation of extant work
- `title` with either CTS URN (extant work) or CITE2URN
- `rs` with `type="waw"` quoted expression not parseable as  a Greek word, e.g. "the letter σ"




### Indexing DSE records

### Indexing dingbats and hyphens



### How to validate


## Editions of scholia

- Erbse
- Dindorf
- Maas
