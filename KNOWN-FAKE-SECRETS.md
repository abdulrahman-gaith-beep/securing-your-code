# Known Fake Secrets Register

> **Audit note:** This file documents secret-looking material that is **intentionally committed** to this repository.
> This repo is the "Securing your code with GitHub" workshop (GitHub Advanced Security training, OWASP Juice Shop sample code).
> Every item below is **dummy / non-functional** lab content used by the secret-scanning exercises (see `_labs/lab5.md`).
> **Do not delete** these files — the lab depends on them. **Do not rotate** them — they are not real credentials.

## Register

| Path | Item (type only — values intentionally omitted) | Why it is present | Rotation note |
| --- | --- | --- | --- |
| `secrets.txt` | Strings formatted like a GitHub Personal Access Token and a Google API key | GHAS workshop lab content (Lab 5 — secret scanning / push protection); dummy, non-functional | Do not rotate — not a real credential |
| `encryptionkeys/premium.key` | Private-key material | GHAS workshop lab content (secret-scanning exercise); dummy, non-functional | Do not rotate — not a real credential |
| `ftp/incident-support.kdbx` | KeePass database file | GHAS workshop lab content (secret-scanning exercise); sample, non-functional | Do not rotate — not a real credential |
| `*.bak` | Backup copies of source/config files | GHAS workshop lab content; intentionally left for scanning exercises | Do not rotate — contains no real credentials |
| `encrypt.pyc` | Compiled Python bytecode | GHAS workshop lab content; part of the encryption/scanning narrative | Do not rotate — contains no real credentials |

## Guidance if this repo is ever reused for real code

If this repository is ever forked, reshaped, or otherwise turned into real production code:

1. **Delete** every file listed above (and any other lab-only artifacts).
2. **Rotate** anything that could possibly be real — treat every committed string as compromised.
3. Keep secret scanning **and** push protection enabled on the new repository.
