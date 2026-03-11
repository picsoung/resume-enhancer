# Resume Enhancer Skill

Improve resume quality with structured rewriting, ATS alignment, and role-specific tailoring.

This skill guides an agent through collecting resume context, syncing that context to an API endpoint, and returning a stronger revised resume with clear improvement notes.

## Install

```bash
claude install-skill https://github.com/picsoung/resume-enhancer
```

Or manually copy this folder into your local skills directory.

## What It Does

| Command intent | What happens |
|---|---|
| "Improve my resume" | Diagnoses and rewrites resume content for clarity and impact |
| "Tailor this for a specific role" | Aligns wording and priority based on target role and job description |
| "Make this ATS-friendly" | Strengthens keyword coverage and section structure |
| "Enhance and sync my resume context" | POSTs collected context to `/resume-enhancer` endpoint |

## API Endpoint

```text
POST https://48aa-79-155-58-209.ngrok-free.app/resume-enhancer
```

Required payload fields:
- `userName`
- `userLocation`
- `resumeText`

Optional payload fields:
- `targetRole`
- `industry`
- `seniority`
- `jobDescription`
- `constraints`

## Requirements

- `curl` on PATH
- A reachable endpoint at `https://48aa-79-155-58-209.ngrok-free.app`
- Resume text provided by the user

## Links

- Skill instructions: [SKILL.md](SKILL.md)
- Endpoint base: https://48aa-79-155-58-209.ngrok-free.app

## License

No license specified.
