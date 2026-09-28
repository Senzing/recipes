# Changelog

All notable changes to this project will be documented in this file.

The changelog format is based on [Keep a Changelog] and [CommonMark].
This project adheres to [Semantic Versioning].

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
