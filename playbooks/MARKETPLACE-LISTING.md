# 🛒 Playbook: MARKETPLACE LISTING | Sage AI

**Owner:** Neve (manager, Venture #4) | **QC:** Echo | **Written:** 2026-10-13 | **Loop:** Assign ➔ Equip ➔ Execute & Self-Correct ➔ Deliver

## 🎯 1. ASSIGN

| Field | Value |
|---|---|
| Owner | Neve |
| Input | An asset that passed QC-AND-DELIVERY |
| Output | A live listing URL logged in `CURRENT-STATE.md` |

**Where this venture sells:**

| Platform | Status |
|---|---|
| Gumroad | Central empire account (Anthony 2026-10-13) |
| Instagram @meet.sage.doula | Posting ON HOLD since 2026-10-11: interview Q1 |
| Sage site (GitHub Pages, docs/) | Public: changes need Anthony OK |
| Amazon.com.au Associates | Account needs Anthony OK |

**Pricing rule:** A$9 to A$35 (deck A$9, journal A$15, partner guide A$19, bundle A$35) per `outputs/BUSINESS-PLAN-LEAN.md`.

## 🧰 2. EQUIP (Toolbox first)

Check `/opt/openclaw/toolbox/INDEX.md` before writing anything new.

| Need | Tool |
|---|---|
| Push listing copy and screenshots to GitHub | `toolbox/scripts/gh_push.py` |
| Check copy before it goes live | `toolbox/formatters/proof_of_done.py` |

## ⚙️ 3. EXECUTE & SELF-CORRECT

1. Listing checklist: title with the buyer's search words, 3 preview images, what's inside, who it's for, A$ price, refund line.
2. Save the copy to `outputs/listings/<slug>.md` and run the Proof-of-Done checker on it.
3. Only list on a platform whose status above is cleared. Anything marked "Anthony OK" goes to Idea Lobster first, once per account.
4. After listing, open the live URL logged out and confirm price, images and delivery work.

## ✅ 4. DELIVER only with proof

1. Run `python3 /opt/openclaw/toolbox/formatters/proof_of_done.py <file> --github clawanthonyzed/sage-ai:<path>@main` and get **0 failures**.
2. The live listing URL opens logged out and shows the right price.
3. `CURRENT-STATE.md` lists the URL.
4. Log: `python3 /opt/openclaw/toolbox/scripts/worklog.py Neve "Sage AI" "<action>" "<GitHub link>"`
5. Report in one line with the clickable GitHub link.

## 📌 Founder Rules (permanent, from Anthony)

| Date | Rule |
|---|---|
| 2026-10-11 | Brand line: Sage Calloway, Virtual Birth Doula & Pregnancy Wellness Companion |
| 2026-10-11 | Sage never claims to be or to have been a midwife |
| 2026-10-11 | Instagram posting waits for Anthony's go-ahead |
| 2026-10-11 | Target A$2,000 per month (AUD) |
| 2026-10-13 | Digital products sell through the central empire Gumroad account |

New rules from [FOUNDER-INTERVIEW.md](https://github.com/clawanthonyzed/sage-ai/blob/main/playbooks/FOUNDER-INTERVIEW.md) are added here, dated, once Anthony answers.
