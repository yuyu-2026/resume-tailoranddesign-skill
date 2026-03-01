# 📄 resume-tailor — Claude Skill

A Claude skill that automatically tailors and rewrites your resume to match a specific job opening. Upload your resume and a job description, and Claude handles the rest: gap analysis, keyword optimisation, ATS compliance, and a polished output in your chosen layout.

---

## What It Does

- **Gap analysis** — compares your resume against the job description, identifying keyword mismatches, buried strengths, and framing opportunities
- **Content rewrite** — rewrites your summary, bullets, and skills section using the employer's exact language, without fabricating anything
- **ATS optimisation** — enforces ATS-safe formatting rules throughout: standard section headers, real selectable text, safe fonts, contact info in the document body, and verbatim keyword matching
- **Four layout options** — keep your existing design, or choose from three professionally designed templates
- **Flexible output** — delivers a `.docx` by default, with optional PDF conversion on request

---

## Layouts

| Option | Description | Best For |
|--------|-------------|----------|
| **A — Keep existing** | Rewrite content only, preserve your current design | Anyone happy with their current layout |
| **B — Two-column professional** | Colored left sidebar with contact & skills; clean right column for experience | Creative, marketing, events, communications |
| **C — Dark sidebar contrast** | Bold name in white on a dark panel; clean white body | Creative directors, copywriters, brand strategists |
| **D — Executive single-column** | Clean, airy single-column with accent rules; authoritative and minimal | Executives, consultants, finance, sales leaders |

---

## How to Install

### Claude.ai (Pro, Max, Team, Enterprise)

1. Download [`resume-tailor.zip`](./resume-tailor.zip) from this repo
2. Go to **claude.ai → Settings → Customize → Skills**
3. Make sure **Code execution and file creation** is enabled under Settings → Capabilities
4. Click **"+"** → **"Upload a skill"** → upload the ZIP

Once installed, Claude will trigger the skill automatically whenever you ask to tailor, optimise, or rewrite a resume for a specific role.

### Claude Code
Add the `resume-tailor/` folder to your project's `.claude/skills/` directory. Claude will discover and use it automatically.

---

## How to Use

Just upload both documents and ask naturally. Example prompts that trigger the skill:

> "Tailor my resume for this job posting"

> "Update my resume to match this job description"

> "Rewrite my CV for this role"

> "Optimize my resume for this application"

**The skill will ask for:**
1. Your current resume (PDF, .docx, or pasted text)
2. The job description (pasted text or URL)
3. Which layout you'd like

Then it delivers a download-ready `.docx`, asks if you'd like a PDF version, and prompts you to add any numbers or metrics that could strengthen the bullets.

---

## ATS Compliance

Every output is built to pass Applicant Tracking Systems:

- ✅ All text is real, selectable text — no images of text
- ✅ Standard section headers (`Experience`, `Skills`, `Education`, `Summary`)
- ✅ Contact information in the document body (not Word header/footer)
- ✅ ATS-safe fonts: Calibri, Arial, Garamond, Georgia
- ✅ Exact keyword matching from the job description
- ✅ Skills listed as plain text, not visual graphics or rating bars
- ✅ `.docx` as the primary output format (safest for ATS portals)

---

## What Claude Will and Won't Change

**Will change:**
- Summary / profile — rewritten to speak directly to the target role
- Bullet framing — reframed using the employer's language
- Skills ordering — most relevant skills surfaced first
- Section structure — optimised for ATS and human readers

**Will never change:**
- Employment dates
- Company names
- Job titles
- Claimed qualifications, degrees, or certifications
- Core facts — only framing and emphasis change, never substance

---

## Requirements

- Claude Pro, Max, Team, or Enterprise plan
- Code execution and file creation enabled in Settings → Capabilities

---

## License

MIT — free to use, adapt, and share.

---

## Contributing

Found a bug or want to suggest an improvement? Open an issue or submit a pull request. If you build on this skill or find it useful, consider submitting it to [awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills).
