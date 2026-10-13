# ✍️ Playbook: CONTENT CREATION | Sage AI

**Owner:** Neve (manager, Venture #4) | **QC:** Echo | **Written:** 2026-10-13 | **Loop:** Assign ➔ Equip ➔ Execute & Self-Correct ➔ Deliver

## 🎯 1. ASSIGN

| Field | Value |
|---|---|
| Owner | Neve (helpers: sage-content-creator, brand-visual-designer, affiliate-research-manager, research-neve, sol) |
| Input | A research file with a Decision (RESEARCH playbook) |
| Output | `outputs/products/<slug>/` (or the venture's existing book / release folder) |

**What this venture makes:**
- Printable cards, guides and journals (A4 + Letter)
- Phone lock screens (1170 x 2532 px)
- Instagram captions with a Meta 'AI info' label on every Sage image (when posting is allowed)
- Gumroad listing copy

**Voice:** Sage Calloway: warm best friend plus calm, knowledgeable guide. Earthy, evidence-based, never clinical or preachy.

## 🧰 2. EQUIP (Toolbox first)

Check `/opt/openclaw/toolbox/INDEX.md` before writing anything new.

| Need | Tool |
|---|---|
| Markdown to print-ready PDF | `toolbox/formatters/md_to_pdf.py` |
| Copy and shot templates | `toolbox/prompt-templates/` |
| Background drafting while the laptop is shut | `toolbox/scripts/queue_task.py` |

## ⚙️ 3. EXECUTE & SELF-CORRECT

1. Write a 5-line brief: goal, buyer, inputs (links), output path, done-when.
2. Build the full asset. Free-route drafts come back in parts of 70 lines or fewer; join them verbatim.
3. Guardrails (any fail = rebuild):
- G1: never a midwife, nurse or any registered practitioner (AHPRA protected titles)
- G2: AI disclosure on every Sage visual (Meta 'AI info' label on posts, a note on products)
- G3: always presented as virtual
- G4: no medical advice; every fact cites RANZCOG, WHO or healthdirect
4. Score against `QC-STANDARD.md`. Below 9.5: name the gap, fix it, score again.

## ✅ 4. DELIVER only with proof

1. Run `python3 /opt/openclaw/toolbox/formatters/proof_of_done.py <file> --github clawanthonyzed/sage-ai:<path>@main` and get **0 failures**.
2. The asset is complete: real copy, real files, no slots left for Anthony to fill.
3. Log: `python3 /opt/openclaw/toolbox/scripts/worklog.py Neve "Sage AI" "<action>" "<GitHub link>"`
4. Report in one line with the clickable GitHub link.

## 📌 Founder Rules (permanent, from Anthony)

| Date | Rule |
|---|---|
| 2026-10-11 | Brand line: Sage Calloway, Virtual Birth Doula & Pregnancy Wellness Companion |
| 2026-10-11 | Sage never claims to be or to have been a midwife |
| 2026-10-11 | Instagram posting waits for Anthony's go-ahead |
| 2026-10-11 | Target A$2,000 per month (AUD) |
| 2026-10-13 | Digital products sell through the central empire Gumroad account |

New rules from [FOUNDER-INTERVIEW.md](https://github.com/clawanthonyzed/sage-ai/blob/main/playbooks/FOUNDER-INTERVIEW.md) are added here, dated, once Anthony answers.
