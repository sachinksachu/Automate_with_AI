# Project rules
- This is a static website: plain HTML, CSS and JS, no framework.
- Entry point is index.html.
- Keep everything in simple, readable files. No new dependencies unless asked.
- After editing, re-read the changed file and check for broken tags, missing closing elements, and accessibility basics (alt text, headings, labels).
- Always run the validation after editing and fix any errors.
- Never commit secrets or API keys.
- Make small, focused changes.


## Review rules

Severity guide:
- high: broken HTML structure, missing alt text, security problems (exposed secrets, unsafe links, inline event handlers with user input), anything that breaks the page.
- medium: accessibility gaps (missing labels, poor heading order, low contrast, missing lang attribute), missing viewport meta tag, broken or placeholder links.
- low: readability problems that make the code hard to maintain.

Do report:
- Problems in lines that were added or changed in this diff.
- Accessibility issues, even small ones.

Do NOT report:
- Formatting, indentation, quote style, or naming preferences.
- Anything html-validate already catches (unclosed tags, missing alt, duplicate IDs), unless it is part of a larger bug.
- Suggestions to add frameworks, libraries, or a build step.
- Issues in unchanged code.
- Vague advice like "consider improving" or "could be better". Every finding must say exactly what is wrong and how to fix it.

Limits:
- At most 3 findings per review. If more exist, keep the most severe.
- Each comment: 1-2 sentences, ending with the suggested fix.
- If the diff only touches docs or config files (README, PROJECT.md, .gitignore), return no findings.