# Documentation language policy (EN / TR)

**Organization:** xrystal-tech  
**Effective:** 2026-11-14

## Principles

1. **User-facing org policy and health files** exist as **paired documents**: English (`.en.md` or default `NAME.md`) and Turkish (`NAME.tr.md` or `policies/NAME.tr.md`).
2. **Both languages have equal authority** for policy text. When updating policy, change both files in the same pull request.
3. **Repository READMEs** in xrystal-tech should provide:
   - English `README.md`, and
   - Turkish `README.tr.md`, **or** a single README with clearly labeled `## English` and `## Türkçe` sections (prefer separate files for longer docs).

## What stays in English only

To keep tooling and APIs stable, the following may remain English-only in application repositories:

- Source code, identifiers, commit messages (English preferred)
- OpenAPI / JSON Schema field names and error codes
- CI workflow and configuration keys

Describe behavior in EN/TR in docs when it affects contributors or users.

## Repository policy docs

| File | English | Turkish |
| --- | --- | --- |
| Repository policy | `policies/repository-policy.en.md` | `policies/repository-policy.tr.md` |
| Privacy policy | `policies/privacy-policy.en.md` | `policies/privacy-policy.tr.md` |

## Review checklist

- [ ] Turkish and English sections convey the same obligations and dates.
- [ ] Links in both files point to the correct paired path.
- [ ] License section matches [repository policy](../../policies/repository-policy.en.md) (default licensed; repo `LICENSE` overrides).