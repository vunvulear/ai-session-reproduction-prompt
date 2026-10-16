# Session Reproduction Package Prompt

A reusable prompt for turning an AI conversation into a documented package that can be reviewed, updated, or reproduced later.

## Why use it

AI-assisted work often depends on more than the final document: source material, evaluation criteria, prompts, decisions, and validation steps all affect the result. This prompt asks an AI assistant to capture those details at the end of a session, so the work can be understood and revisited when new information becomes available.

The package supports transparency and repeatability. It does not guarantee that a future AI run will produce identical results; models, sources, and context may change.

## Files

- [`prepare-session-reproduction-package.md`](prepare-session-reproduction-package.md) — the reusable prompt.

When run, the prompt asks the assistant to create a dated package containing, where available:

- `README.md` — purpose, package contents, and steps for updating or reproducing the work.
- `method.md` — method, criteria, relevant prompts and instructions, decisions, and writing rules.
- `sources.md` — sources and input data, with identifying details and their role in the work.
- `run-log.md` — session date, visible model and tools, key steps, validation, changes, and known limitations.
- A copy of the final output and available raw model outputs, when they can be included without misrepresenting or recreating unavailable material.

## How to use

1. Open the prompt file and copy the text inside its fenced `text` block.
2. Paste it at the end of the AI session that produced the work.
3. Choose one of the delivery options when asked:
   - **Local folder:** provide a folder path where the assistant can save the package.
   - **Downloadable files:** ask the assistant to provide the package for download in the chat.
4. Review the generated package, especially its sources, conclusions, and any items marked unknown or unavailable.

If a folder path or delivery preference has already been stated in the session, the prompt instructs the assistant to use it without asking again.

## Design principles

- Use only information available in the conversation and accessible files.
- Mark missing details explicitly instead of guessing.
- Distinguish source evidence from interpretation and editorial decisions.
- Preserve prompts faithfully and label reconstructed prompts as such.
- Record what should be rechecked during a future update.
- Do not modify or delete source files.
- Do not include secrets or unnecessary personal information.

## Limitations

The prompt can only capture information visible to the assistant or available in files it can access. It cannot recover hidden model settings, unavailable source documents, or raw outputs that were not retained. Future runs may differ even when the same prompt is used.

## Suggested repository layout

```text
.
├── README.md
└── prepare-session-reproduction-package.md
```
