# Contributing to luopan

Thank you for helping. This project is small and its rules are its core asset, so contributions are reviewed carefully.

## What this project values

- **Real-world evidence.** Every rule in `skills/travel-planner/SKILL.md` exists because a real itinerary failed a real need. Proposals for new rules should come with a concrete case: a destination, a scenario, and what the old output got wrong.
- **Neutral wording.** Public copy avoids promotional language and inflated claims. The iteration log records what was tried and what broke; the docs say what the skill does, nothing more.
- **Traceability.** Factual data in itineraries carries sources and query dates. Contributions that weaken this are rejected.

## Reporting issues

Use the issue templates:

- [Bug report](https://github.com/saudademjj/luopan/issues/new?template=bug_report.md): itinerary output that violated a rule, wrong data, or a broken install path
- [Feature request](https://github.com/saudademjj/luopan/issues/new?template=feature_request.md): a new rule idea, a new output section, or a workflow improvement

When reporting an itinerary bug, include: destination, dates, party size, budget tier, and the offending excerpt. That is the same "clean scenario" format used in internal iteration rounds.

## Proposing a rule change

1. Open an issue first, or comment on an existing one, describing the concrete case
2. State what the current behavior produces and what it should produce instead
3. Wait for discussion before opening a pull request. Rule changes are judged against the iteration log, not against preferences

## Pull requests

1. Fork the repository and create a branch
2. Keep changes small: one logical change per pull request
3. If the pull request changes rules or output format, update `ITERATIONS.md` in the same pull request
4. If the change affects installation or usage, update both `README.md` and `README.zh-CN.md`
5. Run a clean test round: prompt a fresh agent with a plain scenario (destination, dates, party, budget) and attach the produced itinerary or research notes to the pull request description
6. Follow the pull request template

### Version policy

Rule or behavior changes bump the version. New rules or output-format changes are `v1.1.0`; fixes are patch bumps. The release process is: update `SKILL.md` and docs, bump the version in the plugin manifest (`plugin.json`), tag, and update `CHANGELOG.md`.

## Code of conduct

All participants agree to follow the [Code of Conduct](CODE_OF_CONDUCT.md).
