````markdown
# Course Build Project

## Purpose

This project uses one master source document to generate multiple course outputs.

The master source document contains:
- course content
- custom structural tags
- file naming instructions
- build notes for AI-assisted processing

This project does not assume that the source document itself is a finished SCORM package.

## Source document

Primary source file:

`source/CP4807 - Introduction to microcontrollers 05 04 26.docx`

## Goal

Use an AI agent plus scripts to:

1. analyse the tagged source document
2. extract content blocks
3. create output files from those blocks
4. assemble learner-facing outputs
5. validate the generated structure
6. package browser and SCORM deliverables where possible

## Project structure

```text
course-project/
├─ source/
│  └─ CP4807 - Introduction to microcontrollers 05 04 26.docx
├─ outputs/
│  ├─ extracted/
│  ├─ docx/
│  ├─ html/
│  ├─ pdf/
│  ├─ browser-course/
│  └─ scorm/
├─ reports/
│  ├─ analysis-report.md
│  ├─ extraction-report.md
│  ├─ validation-report.md
│  └─ packaging-report.md
├─ specs/
│  ├─ tag-rules.md
│  ├─ output-rules.md
│  └─ scorm-rules.md
├─ scripts/
│  ├─ parse_source.py
│  ├─ extract_blocks.py
│  ├─ build_browser_course.py
│  ├─ build_scorm_package.py
│  └─ validate_outputs.py
└─ README.md
````markdown