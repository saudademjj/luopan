# Security Policy

## Supported versions

Only the latest release is supported. Fixes land on the `main` branch and are tagged with the next version.

## Reporting a vulnerability

This repository distributes an instruction file (a skill), not executable code. The relevant risks are:

- **Prompt injection**: content from websites or other untrusted input that tries to override the skill's rules
- **Misleading factual data**: sources that look official but are not
- **Harvesting**: an itinerary that encourages sharing credentials, ID numbers, or payment details

To report a vulnerability or a concern:

1. Open a [private security advisory](https://github.com/saudademjj/luopan/security/advisories/new), visible only to the maintainer
2. Include the trigger scenario, the offending excerpt, and the expected safe behavior
3. Allow up to 7 days for a first response

Do not open public issues for security matters before a fix is released.

## Skill behavior notes

The skill is prompt-level only: it cannot execute code, install packages, or read local files beyond what the client permits. Review `skills/travel-planner/SKILL.md` before installing from any fork or mirror. Only install from this repository or the official release asset.
