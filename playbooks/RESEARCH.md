# 🔬 Playbook: RESEARCH | Sage AI

**Owner:** Neve (manager, Venture #4) | **QC:** Echo | **Written:** 2026-10-13 | **Loop:** Assign ➔ Equip ➔ Execute & Self-Correct ➔ Deliver

## 🎯 1. ASSIGN

| Field | Value |
|---|---|
| Owner | Neve (helpers: sage-content-creator, brand-visual-designer, affiliate-research-manager, research-neve, sol) |
| Run when | Before any new product, book, release or price change |
| Output | `outputs/research/<YYYY-MM-DD>-<topic>.md` |

**Questions this playbook answers:**
- What do first-time pregnant women in Australia ask most, week by week?
- What does an Australian source (RANZCOG, WHO, healthdirect) actually say on that topic?
- Which competing printables and creators exist, at what prices, with what complaints?

## 🧰 2. EQUIP (Toolbox first)

Check `/opt/openclaw/toolbox/INDEX.md` before writing anything new.

| Need | Tool |
|---|---|
| Public web page (blocked or not) | `toolbox/scrapers/stealth_fetch.py <url> --out file.md` |
| Video or post transcript | `toolbox/scrapers/media_ingest.py` (run with its own venv, see INDEX) |
| Turn notes into a PDF | `toolbox/formatters/md_to_pdf.py` |

**Sources for this venture:**
- RANZCOG, WHO and healthdirect pages (cite every fact)
- Public forum threads (read only, never quote private people)
- Etsy and Gumroad search pages (read only)
- `memory/persona/sage-calloway-bible.md` for voice

## ⚙️ 3. EXECUTE & SELF-CORRECT

1. Write the question at the top of the file.
2. Collect evidence: at least 3 sources, each with a working link and the date checked.
3. Put findings in a table: claim, number, source link.
4. End with **Decision**: one recommendation the next playbook can act on, with the reason.
5. Self-check: every number has a source; anything unproven is removed, not guessed.

## ✅ 4. DELIVER only with proof

1. Run `python3 /opt/openclaw/toolbox/formatters/proof_of_done.py <file> --github clawanthonyzed/sage-ai:<path>@main` and get **0 failures**.
2. Every claim in the table has a link that opens.
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
