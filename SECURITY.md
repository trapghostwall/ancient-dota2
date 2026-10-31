# Security policy

## Scope

This repository contains documentation and SVG artwork only. It does not ship a
runtime, loader, DLL, EXE, or game hook. Security reports should concern the
repository itself, for example:

- a malicious link added to the documentation;
- a leaked credential or personal data in an issue or commit;
- an SVG or workflow that can execute untrusted code;
- a supply-chain problem in the validation workflow.

## Reporting

Do not open a public issue for a credential leak or a malicious link. Contact the
maintainers privately through the repository's contact channel and include:

- the affected file or URL;
- a short description of the risk;
- reproduction steps, if safe;
- a suggested fix, if known.

## What not to send

- Passwords, session tokens, Steam Guard codes, or GitHub PATs.
- Full logs containing account identifiers.
- Malware samples or cheat binaries.
- Requests to test anti-cheat evasion.

## Response

Maintainers will acknowledge a report when possible, remove exposed secrets,
and document the fix in the changelog without republishing the secret. There is
no bug bounty and no guarantee of a response time.
