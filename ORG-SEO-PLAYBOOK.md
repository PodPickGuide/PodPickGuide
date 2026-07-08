# GitHub Organization SEO Playbook - PodPick Guide

## Core Idea

GitHub is not only for code. Treat it as a **public database and search entry**.

Google likes structured, citable public data. An Organization has stronger brand entity signals than a personal account.

## Architecture: One Topic Per Repo

```
PodPickGuide (Organization)
|
|-- .github                    Organization profile README
|-- PodPickGuide               Hub index
|-- podpick-flavour-index      Flavour index keywords
|-- vape-comparison-data       Brand comparison keywords
|-- pod-flavour-ranking        Ranking keywords
|-- pod-faq-database           FAQ dataset
|-- pod-buying-guides-data     Buying guide index
```

Never create empty repositories. Every repo should include:
- SEO-ready README (Version / Last Updated / Sources)
- `/data/*.json` machine-readable data
- Cross-links to other repos + podpickguide.com

## README SEO Template

```markdown
# [Target Keyword] - [Subtitle]

## Meta
| Version | 1.0.0 |
| Last Updated | 2026-07-08 |
| Sources | podpickguide.com/... |

## [Data tables]

## Machine-Readable Data
- data/xxx.json

## Related Repositories
```

## GitHub Topics

```
vape, pod-system, flavour-guide, disposable-vape,
sp2s, alibarbar, buying-guide, public-dataset
```

## Current Status

- GitHub Organization `PodPickGuide` created
- 6 topic repositories migrated into the Organization
- Org Profile README deployed (`.github` repo)
- Website cross-link still pending on podpickguide.com

## Website Link

Add footer link:

```html
<a href="https://github.com/PodPickGuide">Data on GitHub</a>
```

Add JSON-LD:

```json
"sameAs": ["https://github.com/PodPickGuide"]
```
