# ChineseStudy reading guides

A small, original reading companion for English-speaking learners interested in Chinese classics. The guides offer reading methods and exercises; the [ChineseStudy reading site](https://chinesestudy.org/) hosts the reading pages they refer to.

Public home: [chinesestudyorg.github.io](https://chinesestudyorg.github.io/).

## Pages

- `/`: English home and guide index.
- `/zh/`: Chinese introduction to the English guides, with a Chinese reading entry.
- `/guides/first-classical-chinese-reading/`: Choose a short passage, read it three times, and keep a focused note.
- `/guides/reading-tang-poetry/`: Follow scene, speaker, and change; try an image map.
- `/guides/tao-te-ching-and-analects/`: Trace a word through a chapter and read a conversation in its situation.

The Chinese home introduces the English guides; it does not present them as translated articles.

## Preview locally

Run from this directory:

```sh
python3 -m http.server 8765
```

Open [localhost:8765](http://localhost:8765/). Root-relative URLs require a server rooted in this directory. No build, JavaScript runtime, package installation, or external font is needed.

## Publish with GitHub Pages

For the account site, use a repository named `chinesestudyorg.github.io`. In the repository settings, choose **Pages → Deploy from a branch → main → / (root)**. Keep `.nojekyll` in the root. No Actions workflow is required.

Canonical URLs, homepage language alternatives, JSON-LD, `robots.txt`, and `sitemap.xml` use `https://chinesestudyorg.github.io/`. If the public hostname changes, update all of them together. Include only real canonical pages in the sitemap. The original guides have no translated equivalents, so they have no translation `hreflang` declarations.

## Editorial and source policy

The prose and reading exercises were written for this guide site. Do not copy reading-site pages, modern translations, or third-party commentary into this repository. Link to a passage in context, and identify the edition or translation when discussing one. Check external links and scholarly claims when updating an article. Do not promise search ranking or imply that an exercise gives a definitive interpretation.

Each guide links to a relevant passage on the official reading site. Only the prominent official reading CTAs use `utm_source=github_pages`, `utm_medium=referral`, `utm_campaign=reading_guides`, and a page-specific `utm_content`. Ordinary references stay clean. Canonical URLs and the sitemap never contain campaign parameters. This site contains no analytics SDK; whether referrals appear in reporting depends on the reading site's existing analytics.

The guides link to [chinesestudy-guide](https://github.com/chinesestudyorg/chinesestudy-guide) for source context and [awesome-chinese-classics](https://github.com/chinesestudyorg/awesome-chinese-classics) for reading resources. Keep those destinations aligned with their actual repository roles.

## Maintenance checks

Before publishing an edit, check the five public pages at mobile and desktop widths, keyboard focus and skip navigation, internal links and section anchors, unique titles and descriptions, JSON-LD, sitemap URLs, and the relevant external reading pages. The layout supports reduced motion and printing. Assets are local; system font availability affects exact glyph shapes.

`assets/social-card.svg` is an editable visual source. A local PNG is used in social metadata only when present; SVG is not declared as an Open Graph image. No license was added. Place any local-only notes in `.local/`, which is ignored by Git.
