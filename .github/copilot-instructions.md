# GitHub Copilot Instructions

## PR Descriptions

When writing a pull request description, act as a P99 principal engineer. Prioritize information density and being easy to scan and grok quickly. Do not state the obvious. Do not justify what does not need justification. Explain clearly in few words as an adept technical leader would.

Structure every PR description as follows:

```
<pr_title>
[concise title]
</pr_title>

<pr_description>
[GitHub markdown body]
</pr_description>
```

### Rules
- Summarize the key points of the problem being solved in 1–2 sentences.
- Describe changes in logical sections using markdown bullet lists with headings.
- Include a code snippet only if it meaningfully illustrates the change.
- Do **not** include test steps, build status, or linting details unless they are part of the problem statement.
- Do **not** include "Fixes #123" or similar issue references — issue linking is handled separately.
- If the PR template contains placeholders like "Fixes [Issue]", remove that section entirely.
- Keep tone informative and professional. Changes still need review — avoid language implying they are final.
