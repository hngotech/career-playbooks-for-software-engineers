**What this does:** Rewrites your resume bullets to improve readability and formatting for recruiters and hiring managers — domain context, compliance frameworks, stakes, and the story of what was broken before you fixed it.

**How to use it:** Upload your current resume to Claude, paste the prompt below into the conversation, and run it.

> **Environment note:** This prompt generates `.docx` and `.pdf` file outputs. It is designed for [Claude](https://claude.ai), which supports code execution. It will not produce downloadable files in environments that do not support it (e.g. ChatGPT, basic API calls).
> 

---

## The prompt

```
# Resume Formatting Prompt — v2

Please reformat the attached resume using the following design system and structure. Generate both a `.docx` and a `.pdf` version as downloadable outputs.

## Design System

Use the `docx` npm library (Node.js) to generate the Word document, then convert to PDF using LibreOffice. Apply these exact style values:

Colors
- Name / Section headers: #000000 (black)
- Body text / Company names: #333333 (dark gray)
- Job subtitles / supporting text: #555555 (medium gray)
- Dates / contact info: #888888 (light gray)
- Hyperlinks: #1155CC (blue)

Typography
- Font: Arial throughout
- Candidate name: size 52, bold, black, centered
- Professional title line: size 24, medium gray, centered
- Contact line: size 19, light gray, centered
- Section headers: size 24, bold, black, ALL CAPS
- Company name: size 22, bold, dark gray
- Job subtitle (title/role): size 20, italic, medium gray
- Dates: size 20, italic, light gray — right-aligned on same line as company via tab stop at position 9360
- Body bullets and skill rows: size 20, dark gray
- Skill row labels: size 20, bold, dark gray

Page Setup
- US Letter: 12240 × 15840 DXA
- Margins: 1080 DXA (0.75 inch) on all sides

Section Dividers
Each section title is a Paragraph with a bottom border: BorderStyle.SINGLE, size 6, navy, space 4. Spacing: 280 before, 80 after.

Bullets
Use LevelFormat.BULLET with a numbering config reference — never unicode bullet characters. Indent: left 480, hanging 240. Spacing: 40 before and after each bullet.
Bullets support an optional bold prefix label (e.g., "Engineering Leadership:") followed by regular-weight body text — use two separate TextRun objects within the same Paragraph.

Skill Rows
Each skill category is a single paragraph: bold label + colon, followed by regular-weight values. Spacing: 60 before and after.

Job Entries
- Company name + right-aligned date on one line (tab stop)
- Job title/subtitle on the line below, italic
- Summary of the company, employee count, product, on the line below, italic
- Followed by bullet points

## Document Structure (Sections in Order)

1. Header — Name, professional title, contact line (location • email • LinkedIn • GitHub)
2. Summary — 3 bullets combining overview narrative and top achievements
3. Core Skills — Skill rows grouped by category
4. Experience — Reverse chronological
5. Selected Prior Experience — Condensed single-line entries for older roles
6. Open Source / Projects — Bold project name, followed by description with repo link

## Summary Section Instructions

Write 3 bullet points total covering the candidate's most impressive technical accomplishments with metrics where available.

## Additional Instructions (Customize Before Running)

- Focus the summary on: [e.g., engineering leadership / product thinking / AI/ML expertise]
- Tailor for this role/company: [paste job description or company name]
- Include or exclude sections: [e.g., remove Open Source section / add Publications section]
- Tone: [e.g., IC-focused, executive-facing, startup-friendly]

## Output Requirements

- Output 1: .docx file — fully formatted per the design system above
- Output 2: .pdf file — converted directly from the .docx
- Filename convention: [FirstName]_[LastName]_Resume_[Version].docx / .pdf
- Do not alter any factual content — only reformat and rewrite the Summary section
- Do not use hard page breaks. Target exactly two pages total.
```

---

*Built by Henry Ngo · Founder, [asmbld](https://asmbld.kit.com/)*
