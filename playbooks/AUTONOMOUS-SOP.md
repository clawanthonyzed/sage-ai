# ⚙️ Autonomous SOP | Sage AI Assembly Line

**Owner:** Neve | **QC:** Echo | **Written:** 2026-10-13 | **Applies to:** every product, caption, image and listing
**Loop:** EXECUTE ➔ TEST ➔ REFINE ➔ SHIP. Nothing skips a station.

---

## 🏭 The Line at a Glance

| # | Station | Agent | Output (saved to) |
|---|---|---|---|
| 1 | 🔬 Ask | research-neve | Audience question + Australian source (`outputs/research/`) |
| 2 | ✍️ Write | sage-content-creator | Product text or caption in Sage's voice (`outputs/content/`) |
| 3 | 🎨 Design | brand-visual-designer | Printable layout / image with AI note (`outputs/products/<slug>/`) |
| 4 | ✅ Test | Echo | Scorecard vs `QC-STANDARD.md` + guardrail check (`outputs/qc/`) |
| 5 | 🔁 Refine | same agent as the fault | v1.1, v1.2 until 9.5+ |
| 6 | 🚀 Ship | Neve | Live Gumroad URL / approved post, logged |
| 7 | 📈 Learn | research-neve | Day-7 keep / fix / kill note |

---

## 1️⃣ EXECUTE

1. Neve reads the week in [90-DAY-AGENT-ROADMAP.md](https://github.com/clawanthonyzed/sage-ai/blob/main/outputs/90-DAY-AGENT-ROADMAP.md) and dispatches:
   - Live: `POST http://localhost:8400/agents/{agent}/tasks/send`
   - Laptop-shut: `python3 /opt/openclaw/orchestration/queue_task.py --agent <agent> --venture "Sage AI" --title "<title>" --brief "<brief>"`
2. Every brief has 5 lines: **goal, reader, inputs (file links), output path, done-when.**
3. Every brief also pastes the 4 guardrails (below) so free-route drafts see them.
4. Free route: about 50 calls a day; ask for parts of **70 lines or fewer**. Layout and image work needs a full-tool session.

## 2️⃣ TEST (Echo): the guardrail check comes first

| # | Guardrail | Fail if |
|---|---|---|
| G1 | 🚫 Protected titles | Sage is called, or implied to be, a midwife, nurse, doctor or any registered practitioner |
| G2 | 🤖 AI disclosure | A Sage image has no AI note (product) or the Meta "AI info" label is off (post) |
| G3 | 🪪 Virtual | Copy suggests Sage is a real person, has real clients or attended real births |
| G4 | 🩺 No medical advice | Any diagnosis, dosage, "you should" medical instruction, or a fact with no RANZCOG / WHO / healthdirect source |

Any G-fail = automatic reject, whatever the score. Then score `QC-STANDARD.md` (9.5 minimum), stop-slop PASS, no em dashes, A$ prices.

## 3️⃣ REFINE

1. Echo writes each gap as **where ➔ problem ➔ fix.**
2. Rework goes to the **same agent**. Neve never quietly rewrites it.
3. Two fails in a row = Neve rewrites the brief, then rebuild.

## 4️⃣ SHIP

1. ✅ Gumroad: central empire account (Anthony 2026-10-13). Neve can list a product that passed Echo.
2. 🛑 Instagram, Pinterest, site changes, Amazon Associates: wait for Anthony's go-ahead. Posting is on hold since 2026-10-11.
3. Every product listing ends with: "General information only, not medical advice. Talk to your midwife, GP or obstetrician. Sage Calloway is a virtual, AI-created companion."
4. Log it:
   `| [YYYY-MM-DD HH:MM AWST] | Neve | Sage AI | Shipped <item> at A$<price> | <link> |`

---

## 🧭 Daily Rhythm (Neve)

| When | Do |
|---|---|
| 🌅 Start | Read `memory/README.md`, persona bible, `CURRENT-STATE.md`, last 20 work-log rows |
| ☀️ Mid | Inspect drafts, run guardrails + QC, send rework |
| 🌙 End | Update `CURRENT-STATE.md`, one work-log line per finished task |

## 🚨 Escalate to Idea Lobster when

- 🩺 A health question can't be answered from a cited source
- 💳 Money, 🔑 accounts, ⚖️ legal or 📸 posting come up
- 📉 0 sales 14 days after a launch
