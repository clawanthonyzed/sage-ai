# 🧪 Playbook: QC AND DELIVERY | Sage AI

**Owner:** Neve (manager, Venture #4) | **QC:** Echo | **Written:** 2026-10-13 | **Loop:** Assign ➔ Equip ➔ Execute & Self-Correct ➔ Deliver

## 🎯 1. ASSIGN

| Field | Value |
|---|---|
| QC owner | Echo (backup: the venture's qc rubric agent) |
| Delivery owner | Neve |
| Standard | `QC-STANDARD.md` (9.5 minimum, flagship 10) + `/opt/openclaw/orchestration/PROOF-OF-DONE-STANDARD.md` |

## 🧰 2. EQUIP (Toolbox first)

Check `/opt/openclaw/toolbox/INDEX.md` before writing anything new.

| Need | Tool |
|---|---|
| Automatic Proof-of-Done checks | `toolbox/formatters/proof_of_done.py <file> --github <repo>:<path>@<branch>` |
| Push and verify on GitHub | `toolbox/scripts/gh_push.py` |
| Work-log row | `toolbox/scripts/worklog.py` |

## ⚙️ 3. EXECUTE & SELF-CORRECT

**Venture checks (any fail = reject):**
- Guardrails G1 to G5 checked before any score; any fail = reject
- Meta 'AI info' label switched on for photorealistic posts
- Ad / affiliate marking present on every promotional post

**Universal checks:** no placeholders, no em dashes, no AI buzzwords, all links open, code and data ran with 0 errors, A$ prices.

**Rework rule:** Echo writes each gap as *where ➔ problem ➔ fix* and sends it back to the agent that made it. Two fails in a row = rewrite the brief, then rebuild.

## ✅ 4. DELIVER only with proof

1. Run `python3 /opt/openclaw/toolbox/formatters/proof_of_done.py <file> --github clawanthonyzed/sage-ai:<path>@main` and get **0 failures**.
2. The file is committed to `clawanthonyzed/sage-ai` and the checker confirms it on GitHub.
3. Only now may Anthony be told, and only with the link.
4. Log: `python3 /opt/openclaw/toolbox/scripts/worklog.py Neve "Sage AI" "<action>" "<GitHub link>"`
5. Report in one line with the clickable GitHub link.

## 🚨 Escalate to Anthony (via Idea Lobster) only for

- 💳 Money, 🔑 accounts, ⚖️ legal
- ❓ A fact only Anthony knows: add it to `FOUNDER-INTERVIEW.md` as a new question, never guess

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
