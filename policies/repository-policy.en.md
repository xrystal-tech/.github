# Repository policy — Xrystal (xrystal-tech)

**Effective:** 2026-11-14  
**Scope:** All repositories under the `xrystal-tech` GitHub organization unless a repository explicitly overrides this policy.

## 1. Purpose

This policy keeps xrystal-tech repositories consistent, legally clear, and accessible to contributors in English and Turkish.

## 2. Licensing (default: licensed)

Unless stated otherwise for a specific repository:

1. **Every public repository must ship with a license file** at the repository root: `LICENSE` or `LICENSE.md`.
2. **Org default license** is the [MIT License](../license-templates/LICENSE-MIT). Use this template when creating a new repository and no other license has been approved for that project.
3. **Repository override:** If the repository root already contains `LICENSE` or `LICENSE.md` that names a different license (for example Apache License 2.0, GPL-3.0, or a custom SPDX identifier documented in the file), **that repository’s license file is authoritative** for that repository. Org defaults do not replace it.
4. **Private repositories** must still document licensing intent in the README (who may use the code and under what terms). If the repo is later made public, add a proper `LICENSE` before changing visibility.
5. **No license / “all rights reserved”** is allowed only when explicitly documented in that repository’s README and approved by org owners (exception path—not the default).

### Quick reference

| Situation | What to do |
| --- | --- |
| New repo, no special instruction | Add org default MIT from `license-templates/LICENSE-MIT` |
| Repo already has `LICENSE` | Keep and honor that file; mention it in README |
| You were told to use another license in that repo | Use that license in `LICENSE` and note it in README |

## 3. Required repository hygiene

Public repositories should include:

- `README.md` (see [i18n policy](../docs/i18n/POLICY.en.md))
- `LICENSE` or `LICENSE.md` (unless a documented private exception)
- Security contact via org [SECURITY.md](../SECURITY.md) or a repo-local `SECURITY.md` only if it **extends** (not contradicts) the org policy

Recommended:

- `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md` (org defaults apply from `.github` repo)
- Issue and pull request templates from `.github`

## 4. Naming and visibility

- Repository names: lowercase, hyphen-separated (`my-service`), unless a published product name requires otherwise.
- Default visibility for new work: follow org owners’ decision (private until ready for public release, unless the project is explicitly open from day one).
- Archived repositories: mark as archived in GitHub settings; keep `LICENSE` in place for historical compliance.

## 5. Dependencies and compliance

- Do not commit secrets, production credentials, or personal data unrelated to the project.
- Third-party code must respect its licenses; document notable obligations in README or `NOTICE` when required (for example Apache-2.0).

## 6. Overrides

A repository may document exceptions in `POLICY.override.md` at its root, linked from README, covering only:

- License choice (must still have a root `LICENSE` or `LICENSE.md`)
- Stricter security or contribution rules

Org-wide policies in this repository still apply where not explicitly overridden.

## 7. Changes

Proposed changes to this policy: issue or PR in `xrystal-tech/.github`, with updates in **both** English and Turkish policy files.