# Validation Report

## Build Status

- Command: `make all`
- Status: Passed
- Output PDF: `compiled/mohnish-shende-cybersecurity-cv.pdf`
- Final PDF synced to: `final.pdf`

## Page Count

- Page count: 2
- Source: `pdfinfo compiled/mohnish-shende-cybersecurity-cv.pdf`

## Warnings And Layout Log

- Overfull boxes: none found
- Underfull boxes: none found
- LaTeX/package warnings: none found by log scan
- Orphaned headings: none observed in rendered PNG review
- Awkward page breaks: none requiring correction; Nmap LLM begins page 2 as the natural continuation of the projects section
- Unbalanced whitespace: acceptable for a two-page technical CV

## `pdftotext` Result

- Extracted text file: `compiled/cv.txt`
- Private-use glyphs: none found
- Replacement/corrupt glyph markers: none found
- Broken hyphens: none observed in checked terms such as `CERT-In`, `self-hosted`, `access-control`, `client-server`, `Zero-Knowledge`, and `NIST SP 800-61`
- Corrupted parentheses: none observed in checked terms such as `(IBI)`, `(tracemalloc)`, and `(Ollama/Mistral)`
- Stray empty bullets: none found
- Reading order: correct single-column order from header, summary, experience, skills, projects, publication, research, and education

## Font Embedding

`pdffonts` confirmed embedded and subset fonts:

- `Inter-ExtraBold-Identity-H`: embedded yes, subset yes, Unicode yes
- `Inter-Regular-Identity-H`: embedded yes, subset yes, Unicode yes
- `LMMono10-Regular-Identity-H`: embedded yes, subset yes, Unicode yes

## Hyperlink Check

PDF URI annotations were found for:

- `mailto:mohnishshende4@gmail.com`
- `tel:+917020172261`
- `https://linkedin.com/in/mohnishshende`
- `https://github.com/MohnishShende`
- `https://scholar.google.com/citations?user=Qu1HDUIAAAAJ&hl=en`
- `https://orcid.org/0009-0000-9466-3056`
- `https://github.com/MohnishShende/NodeZero`
- `https://github.com/MohnishShende/IBI-schemes`
- `https://github.com/MohnishShende/nmap-llm`
- `https://doi.org/10.1080/24732850.2025.2599908`
- `https://github.com/MohnishShende/somerton-man-intelligence-dossier`

Network spot check:

- GitHub profile: 200
- Google Scholar: 200
- ORCID: 200
- NodeZero repository: 200
- IBI Schemes repository: 200
- Nmap LLM repository: 200
- Somerton Man repository: 200
- LinkedIn: 999 from automated curl, consistent with bot blocking; PDF annotation is present
- DOI: resolves to Taylor & Francis, then returns 403 to automated curl; PDF annotation is present

## Visual Inspection

- Rendered pages inspected:
  - `compiled/review/cv-page-1.png`
  - `compiled/review/cv-page-2.png`
- No clipped text, overlapping text, unreadable glyphs, orphaned section headings, or broken section hierarchy observed.
- Header remains compact with profile labels.
- Technical Skills remain visible on page 1 before projects.
- New responsible disclosure and Somerton Man bullets remain readable on page 2.

## Final ATS Assessment

ATS readability is strong. The document is single-column, uses conventional section headings, preserves searchable cybersecurity keywords, keeps skills early, avoids private-use glyph extraction, and exposes link labels in the text layer with valid PDF URI annotations. The main tradeoff is that compact profile labels do not expose full profile URLs in extracted text, but the clickable annotations are present and the labels are clear to human reviewers.
