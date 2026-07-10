# Release Report v1.0.0

## Repository

- Repository URL: https://github.com/MohnishShende/professional-portfolio
- Release commit SHA: `4a8f156c0f34f12daaaaa13016603fb6a411fa96`
- Tag: `v1.0.0`
- Release URL: https://github.com/MohnishShende/professional-portfolio/releases/tag/v1.0.0
- Release asset: `cybersecurity-cv-v1.0.0.pdf`
- Release asset SHA-256: `b4e771be7c171d7a0a05c86661237588ab8849764cbd1a34512c7ccb7c0aa9d8`

## Included Files

- `README.md`
- `LICENSE-NOTICE.md`
- `CHANGELOG.md`
- `.gitignore`
- `release_notes_v1.0.0.md`
- `cv/cybersecurity/README.md`
- `cv/cybersecurity/Makefile`
- `cv/cybersecurity/cv.tex`
- `cv/cybersecurity/style/shendecv.sty`
- `cv/cybersecurity/sections/summary.tex`
- `cv/cybersecurity/sections/experience.tex`
- `cv/cybersecurity/sections/skills.tex`
- `cv/cybersecurity/sections/projects.tex`
- `cv/cybersecurity/sections/publication.tex`
- `cv/cybersecurity/sections/research.tex`
- `cv/cybersecurity/sections/education.tex`
- `docs/change_report.md`
- `docs/validation_report.md`
- `docs/release_validation_v1.0.0.md`
- `docs/privacy_audit_v1.0.0.md`
- `releases/cybersecurity-cv-v1.0.0.pdf`

## Excluded Sensitive Categories

- Degree certificates
- Identity documents
- Appointment letters
- Private evidence files
- CERT-In email correspondence
- Full private security reports
- Internal notes containing sensitive information
- Temporary build files
- LaTeX auxiliary files
- Local absolute paths
- API keys, tokens, credentials, and secrets
- Screenshots containing personal or private information
- Drafts not intended for public release
- Duplicate or obsolete CV directories

## Build Verification

- Build command: `cd cv/cybersecurity && make all`
- Build result: passed
- Page count: 2
- Text extraction: clean
- Font embedding: Inter and LMMono fonts embedded, subset, and Unicode mapped
- Visual review: passed
- Hyperlink annotations: present for email, phone, professional profiles, project repositories, DOI, and Somerton Man repository

## Privacy Audit Result

The v1.0.0 public file set was scanned for identity-document terms, credentials, private keys, API tokens, CERT-In email bodies, local absolute paths, and sensitive disclosure records. No private evidence, credentials, identity documents, or sensitive disclosure correspondence were found.

## Fresh-Clone Test Result

A fresh clone from `https://github.com/MohnishShende/professional-portfolio.git` built successfully from `cv/cybersecurity` with `make all`.

Fresh-clone validation:

- Page count: 2
- Fonts embedded: yes
- Private-use glyphs: none found
- Replacement characters: none found
- Empty bullets: none found
- Build artifacts are generated locally and ignored by `.gitignore`

## Unresolved Limitations

- The release PDF and a newly built PDF have different SHA-256 values because XeLaTeX writes nondeterministic PDF metadata. Their extracted text is identical and visual rendering was inspected.
- LinkedIn returned HTTP 999 to automated curl checks, consistent with bot blocking. The PDF annotation and README URL are present.
- The DOI resolves to Taylor & Francis and returned HTTP 403 to automated curl checks, consistent with publisher bot blocking. The DOI annotation and README URL are present.
- This report was generated after the GitHub Release existed so it could include the final release URL and asset metadata.
