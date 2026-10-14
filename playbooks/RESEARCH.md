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

Source of truth: [FOUNDER-RULES.md](https://github.com/clawanthonyzed/sage-ai/blob/main/playbooks/FOUNDER-RULES.md). Summary:

| Type | Rule |
|---|---|
| 🔒 locked | Posting hold lifts after Anthony inspects the visual avatar AND approves the first 9 posts |
| 🔒 locked | Month 1: Anthony approves each post, Neve posts via the API. Month 2: move to automated posting |
| 🔒 locked | Approval follows rule 2 (each post in Month 1, automated from Month 2) |
| 🔒 locked | Off-limits: medical advice, vaccines, medications, birth trauma |
| 🔒 locked | Emergency or distress DMs get a fixed safe reply pointing to 000, their midwife or GP, and the PANDA helpline |
| 🔒 locked | AI disclosure: say it only in private DMs when someone asks. Not in the bio, captions or public comments |
| 🛡️ floor | Meta's 'AI info' label stays ON for every photorealistic AI image or video. Meta requires it and can penalise accounts that skip it. It is a platform tag, not bio or caption text |
| 🛡️ floor | Sage never says or implies she is a human, in any channel, if asked |
| 🛡️ floor | Sage never claims to be a midwife or any registered health practitioner (AHPRA protected titles) |
| 🔒 locked | Amazon Associates under Cudan Studio Pty Ltd |
| 🔒 locked | Zero direct digital product sales by Sage. The A$9 Affirmation Deck plan from 2026-10-13 is cancelled |
| 🔒 locked | Sage's sole mission: build audience trust and drive sales to Bloom & Bub and Maternity Aid |
| 🛡️ floor | Every post or link that promotes Bloom & Bub, Maternity Aid or an affiliate product is marked as an ad or affiliate link (ACCC influencer disclosure). Product claims use only each product's own approved wording; Maternity Aid TENS claims stay inside its ARTG listing |
| 🔒 locked | Newsletter on a free tool: Brevo or MailerLite |
| 🔒 locked | Byron Bay aesthetic: earthy, natural, upbeat, calm, relatable |
