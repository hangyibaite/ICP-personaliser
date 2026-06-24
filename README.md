# ICP-personaliser

A Claude skill that builds a hyper-specific Ideal Client Profile through guided conversation.

## What it does

Runs a structured interview to extract a complete ICP from anyone — even if they don't know their ICP yet. Handles vague answers, challenges contradictions, and produces a tailored markdown document.

## Structure

```
ICP-personaliser/
├── SKILL.md                  # Main skill — core rules and flow
├── README.md                 # This file
├── output-format.md          # Standardised ICP output structure and template
├── synthesis.md              # Rules for summarising and confirming back
└── references/
    ├── question-framework.md # Full 10-round questioning sequence
    └── ambiguity-handling.md # 8 techniques for handling vague/confused answers
```

## Installation

Add this folder to your Claude project's skills directory, or upload it as a custom skill.

## Usage

Tell Claude: "Help me define my ICP" or "Build my ideal client profile."

The skill will run a multi-round interview, confirm each section, and generate a single markdown ICP document tailored to your business.
