# Command: Prepare a Session Reproduction Package

Copy and run the command below at the end of an AI session in which you produced a report, research, analysis, or other material that you may want to update or reproduce later.

```text
Prepare a reproduction package for this session.

SAVE LOCATION AND DELIVERY
If I have already specified a local folder path or asked for downloadable files, use that preference without asking again. Otherwise, ask me to choose one:
1. Local folder — ask me for the folder path, then save the package there.
2. Downloadable files — create the package and provide it for download in this chat.

Do not assume you can write to a local folder unless the current environment supports it. If the chosen option is unavailable, explain the limitation and offer the other option. If neither file creation nor downloads are available, provide the package contents in the conversation.

Create a new package folder named YYYY-MM-DD_<short-topic>. For local saving, place it under the folder path I provide. For downloads, create the package in an available workspace and provide it as a ZIP file; if ZIP creation is unavailable, provide the files individually. Never overwrite an existing package. If the name is already in use, add a numeric suffix. Use the current date available in the session.

PURPOSE
Extract information from the current conversation and available files that will help someone understand how the material was produced and update or reproduce it using new data.

FILES TO CREATE
1. README.md — the purpose, package contents, and recommended steps for updating or reproducing the work.
2. method.md — the method, criteria, requested structure, relevant prompts and instructions, decisions made, and writing rules.
3. sources.md — the sources and input data used, including title, URL or location, date/version, and role in the analysis where available.
4. run-log.md — session date, tools and model only if visible, key steps, validations performed, changes from previous versions, and known limitations.
5. Include a copy of the session's final output in an appropriate format only if the output is available as a file or can be saved without changing its content. Preserve its suitable extension and formatting. If it is not available, say so in README.md; do not recreate it and label it as the original.
6. If raw model outputs distinct from the final output are available in the conversation or files, save them separately and describe them in README.md. Do not recreate raw outputs that are no longer available.

EXTRACTION AND ACCURACY RULES
- Use only information present in the conversation or in files you can access. Do not invent sources, prompts, steps, results, model versions, or settings.
- Explicitly mark unavailable information as “Unknown” or “Not present in the conversation.” Distinguish confirmed information from assumptions.
- Preserve important prompts and instructions as faithfully as possible. If you reconstruct a prompt from multiple messages, label it “Reconstructed” and note what cannot be verified.
- Link important conclusions to the sources or evidence that support them where identifiable. Separate source facts from interpretations, recommendations, and editorial decisions.
- Note what should be replaced or rechecked during the next update, including information that may change over time.
- Do not claim that a future run will produce an identical result. Briefly explain that the model, sources, and context may change.
- Do not include secrets, passwords, access keys, or unnecessary personal data. If materials contain sensitive data, identify the affected material and redact only what is necessary in the package. Do not alter source files.
- Save or provide only the package files. Do not modify or delete source files or other existing files.

FINAL CHECK
Verify that every created file is present and readable. Then confirm in the conversation whether the package was saved locally or provided for download, give its full folder path or download link(s), list the included files, and note any important information that remained unknown or could not be saved.
```
