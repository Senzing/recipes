# Changelog

All notable changes to this project will be documented in this file.

The changelog format is based on [Keep a Changelog] and [CommonMark].
This project adheres to [Semantic Versioning].

## [1.3.0] - 2026-09-28

### Changed in 1.3.0

- Recipe intros rebuilt around the reader's decision: what you'll build, what it takes, the
  screenshot with its numbers, then the demo link. Each opens with the general case and hands off to
  the sample data, so the claim transfers to your own
- **What it takes** sits above the screenshot as one scannable line - level, how long once you're
  set up, where it runs, anything needed first - instead of below the video
- Every prompt is introduced with "Paste this into your AI assistant", and every step opens with how
  many prompts it holds. One recipe previously went straight from a heading into a bare code block
- **Before you begin** is its own section between Setup and the first step, replacing a blockquote
  at the end of Setup that GitHub rendered as a muted aside
- Each recipe ends with the same **Next** line, sending the reader back to the cookbook to pick
  another; choosing one is the catalog's job
- Horizontal rules removed; GitHub already draws one under every heading
- The cookbook page opens with what these demos are and what builds them - Senzing, its MCP, and
  your own AI assistant - and defines what Easy, Intermediate and Advanced mean
- Possible matches are described as pairs that call for a human decision, not ones Senzing was
  unsure about
- Step introductions say what the step does rather than how its prompt was written. "This is the
  loader - cook it properly" and "the loader must be production-grade" were notes to the author;
  they now tell the reader what happens, including that the AWS build pauses part-way for approval
- Kitchen and place-setting vocabulary is gone from reader-facing prose. It was defined only in
  files that never published, so it meant nothing on the page

### Fixed in 1.3.0

- *Find the Entities Hiding Across Your Data* combines three sources, not two; the intro said two
  and the third arrives in its final step

### Added to 1.3.0

- A fourth reminder in every recipe on how to ask the assistant what went wrong: describe the gap,
  tell it to verify rather than guess, and don't start over

### Renamed in 1.3.0

- *Combine Data Sources & Explore Hidden Connections in PPP Loan Data* is now
  **Find the Entities Hiding Across Your Data**. The old title named the sample data rather than
  what the recipe shows; the page slug is unchanged

## [1.2.0] - 2026-09-28

### Changed in 1.2.0

- Recipe front matter trimmed to the fields that do work: `title`, `use_case`, `difficulty`,
  `est_time`, `video`, `author`. Dropped `id`, `type`, `languages`, `kitchen`, `place_setting`,
  `version` and `senzing_version`, and with them the per-recipe Changelog sections
- Front matter now ships with the recipes instead of being stripped on publish, so the metadata
  the website build parses is present in this repo
- Use case is the only filter the catalog offers; difficulty, platform and time stay on each
  catalog line as plain text
- Retired the "Optional refinements" section, which only Customer 360 used

### Fixed in 1.2.0

- Healthcare Exclusion Screening links its demo on YouTube rather than a temporary Google Drive copy
- Combine Data Sources & Explore Hidden Connections in PPP Loan Data links its own demo; it had been
  pointing at a different recipe's video

## [1.1.0] - 2026-09-08

### Added to 1.1.0

- Stewardship on CRM + Online Orders: a recipe that adds a data stewardship queue to the
  Customer 360 app, so a human can review possible matches and decide Merge or Don't merge

### Changed in 1.1.0

- Dropped the "Questions that may come up" sections from every recipe

## [1.0.0] - 2026-08-14

### Added to 1.0.0

- Initial content: the Senzing Cookbook, Get Started, three recipes, and a synthetic
  Customer 360 ingredient set

[CommonMark]: https://commonmark.org/
[Keep a Changelog]: https://keepachangelog.com/
[Semantic Versioning]: https://semver.org/
