# Changelog

All notable changes to luopan are recorded here. Versions follow SemVer.

## [1.1.0] - 2026-08-10

### Changed

- Skill: requirements gathering adds departure city (affects transport and budget baseline, with the assumption noted in output header)
- Skill: budget refusal fallback — if the user declines to state a budget, default to the comfort tier and note it in the output header
- Skill: R6 wording tightened (宁可排松)
- Landing page: full redesign in the personal-site design language — dark glassmorphism, compass motif with a slow rotating dial, grid-and-noise texture
- Landing page: WCAG AA contrast fixes for buttons, links, index labels and tint cards, in light and dark themes
- Search discoverability: bilingual repo description, homepage link, 10 topics, JSON-LD structured data on the landing page, richer marketplace description
- Code of conduct replaced with the standard Contributor Covenant v2.1 text
- English README wording tightened

### Added

- English README, with the Chinese version split into `README.zh-CN.md`
- Community files: `CONTRIBUTING.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`, issue and pull request templates, `CHANGELOG.md`

## [1.0.0] - 2026-08-07

Initial release.

### Added

- Skill: budget gate, scope red line, source hierarchy with query dates, workload-by-scale rules, pre-delivery self-check table
- Plugin distribution: plugin manifest (`plugin.json`) and marketplace manifest (`marketplace.json`), two-command install
- Docs: GitHub Pages landing page at https://saudade.me/luopan/
- Iteration log with rules and verification rounds across Nanjing, Suzhou, Hangzhou, Beijing and a Xinjiang self-drive trip
- Example output: 10-day Xinjiang self-drive loop
- MIT license

[1.1.0]: https://github.com/saudademjj/luopan/releases/tag/v1.1.0
[1.0.0]: https://github.com/saudademjj/luopan/releases/tag/v1.0.0
