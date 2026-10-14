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
| Instagram @meet.sage.doula | Hold lifts after Anthony inspects the avatar and approves the first 9 posts; Month 1 Anthony approves, Neve posts via API; Month 2 automated |
| Newsletter (Brevo or MailerLite, free tier) | Approved |
| Amazon.com.au Associates | Approved under Cudan Studio Pty Ltd |
| Bloom & Bub + Maternity Aid shops | Where Sage sends buyers; their managers own the listings |

**Pricing rule:** Sage sells nothing directly (Founder Rule 9). Success = trusted audience + referred sales.

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
