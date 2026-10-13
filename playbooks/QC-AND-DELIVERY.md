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
- Guardrails G1 to G4 checked before any score; any fail = reject
- Disclaimer line on every product and listing
- Prints on home A4 with no clipping

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

| Date | Rule |
|---|---|
| 2026-10-11 | Brand line: Sage Calloway, Virtual Birth Doula & Pregnancy Wellness Companion |
| 2026-10-11 | Sage never claims to be or to have been a midwife |
| 2026-10-11 | Instagram posting waits for Anthony's go-ahead |
| 2026-10-11 | Target A$2,000 per month (AUD) |
| 2026-10-13 | Digital products sell through the central empire Gumroad account |

New rules from [FOUNDER-INTERVIEW.md](https://github.com/clawanthonyzed/sage-ai/blob/main/playbooks/FOUNDER-INTERVIEW.md) are added here, dated, once Anthony answers.
