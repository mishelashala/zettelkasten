---
status: someday
created: 2026-10-10
tags: [project, runes, typography, vscode]
---

# RuneSmith

Personal tools for reading and writing runes comfortably in an editor.

**Status:** Future project — revisit when time permits.

## Motivation

The current appearance of Unicode runes in my editor is unsatisfactory. I want better typography and writing assistance that makes runic text easier to compose, check, and read.

## Idea 1: A Futhark font for my editor

Create a font with attractive, legible Futhark glyphs mapped to the existing Unicode runic characters.

- Consistent stroke weight, spacing, and alignment.
- Clear shapes at everyday editor sizes.
- Editor-friendly metrics, ideally monospaced.
- Preserve the underlying Unicode text so files remain portable.

Decide later which Futhark variant to support first, and whether to include the additional Anglo-Saxon Futhorc characters needed by the extension.

## Idea 2: An Anglo-Saxon rune assistant for VS Code

Create a VS Code extension that acts as a spell checker for English written with Anglo-Saxon runes (Futhorc).

- Recognize runic words in a document.
- Flag likely spelling or rune-selection mistakes.
- Offer “Did you mean…?” suggestions and a way to apply corrections.
- Hover over a runic word to see its English spelling and pronunciation.
- Display pronunciation using Merriam-Webster-style notation.

Example interaction: write the runic equivalent of **show**, then hover over it to see **show** and its dictionary pronunciation.

## Questions to settle when starting

- Is the writing system for modern English rendered in Futhorc, historical Old English, or separate modes? The English-word hover example suggests modern English as the initial use case.
- What spelling or sound-to-rune conventions should the spell checker accept?
- How should ambiguous rune sequences and multiple candidate words appear?
- Which dictionary and pronunciation source can be used, and under what terms?
- Should single-rune hovers also show the rune name and sound values?

## First steps

- [ ] Collect examples of the current font problems.
- [ ] Choose an initial rune inventory and writing convention.
- [ ] Sketch a small set of glyphs and try them in the editor.
- [ ] Prototype runic-word recognition and an English-word hover.
- [ ] Add correction suggestions after the mapping works reliably.
