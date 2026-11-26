# Language Prompt

> **Repository rename TODO:** Rename this GitHub repository from `sinukus/Language-Template` to **`sinukus/Language-Prompt`** under **Settings → General → Repository name**. Update links, remotes, and downstream references after renaming.

## Purpose

Language Prompt is the **human-editable, English-only Markdown source of truth** for the language questions, topics, and communication needs that Travel Expert uses. The prompts and category descriptions are authored in English; translated phrases, pronunciation, and explanations are generated for the traveler's target language downstream.

The original language content was previously consolidated into [Travel Expert's `language/` directory](https://github.com/sinukus/travel-expert/tree/main/language) (import revision `7f1a5b858b3d86c465da30512be974f920090926`, consolidation commit `e74bbb1bc0b0d3a24f2748a29c7fd467726282d7`). **That historical consolidation must be reconciled before this repository becomes the authoritative active source again.** Do not silently overwrite or duplicate later changes made inside Travel Expert.

## Authoring principles

- Keep all source questions, section titles, and instructions **in English**.
- Use straightforward Markdown that can be corrected in any text editor.
- Organize content into independently optional interest sections, each with a stable ID; retain all existing questions when reorganizing.
- Keep common safety and emergency language available regardless of optional topic selections.
- Keep Travel Expert's runtime, translation, pronunciation, data-source adapters, and user interface separate from the authored prompts.
- Derive machine-readable outputs from Markdown using a validated build step; do not hand-maintain a competing JSON source.

## Suggested sections (not yet migrated)

- Greetings and social conversation
- Food and drink
- Transport and directions
- Accommodation
- Shopping, prices, and bargaining
- Health, emergencies, and accessibility
- Local etiquette and practical phrases
- Face-to-face conversation

## Migration TODO

1. Audit the original language prompt and the current `travel-expert/language/` tree, preserving edits made since consolidation.
2. Restore the full canonical English prompt content here as editable Markdown.
3. Add stable section IDs and optional-interest metadata without losing existing content.
4. Validate and generate application-consumable data from the Markdown.
5. Change Travel Expert to consume generated artifacts rather than maintaining an independent source.
6. Rename this repository to `Language-Prompt`, then update repository links and references.

**Status:** This README documents the agreed direction. The source migration, parser, integration, and repository rename are not yet complete.
