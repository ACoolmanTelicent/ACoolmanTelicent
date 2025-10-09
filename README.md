- 👋 Hi, I’m @ACoolmanTelicent
- 👀 I’m interested in making pedestrian things automated, and valuable problems front and center
- 🌱 I’m currently learning about home labbing
- 💞️ I’m looking to collaborate on DX
- 📫 How to reach me is MS Teams

# On communication style

I'll try and be precise by default.

But if I can't think of anything better to do, I'll end up _biasing toward action_ BUT with some time, care and effort put aside for cleaning up any confusion I cause.

# Docs & process — the pantheon (aim & cost)

**Assume zero comments.** Make the thing clear enough that nothing needs explaining.  
**Code is written once, read many times** ([why readability matters](https://martinfowler.com/bliki/CodeAsDocumentation.html)).

---

## 🏆 BEST — No reading needed
- Automate the step; make the UI/CLI guide the next action ([toil → automate](https://sre.google/sre-book/toil/)).
- **Cost later:** lowest. Nothing to maintain.

## 👼 OK — In-flow cues (just-in-time)
- Short hints and error remedies at the point of failure ([contextual help](https://www.nngroup.com/articles/contextual-help/)).
- **Cost later:** low. Lives next to the code/path.

## ✅ OK — Process aids (tight, execution-focused)
- Small checklists, scripts, or templates for repeatable work (e.g., “integration setup”, “run this meeting”).
- Prefer executable or templated forms over prose ([checklists work](https://www.nejm.org/doi/full/10.1056/NEJMsa0810119)).
- **Cost later:** low–medium. Tied to workflow; easy to version with the thing it supports.

## 📜 RISKY — Long guides / narratives
- Multi-page “how it works” or policy write-ups.
- **Cost later:** high drift, search friction, easy to misread. Use only when shorter forms cannot do the job.

## ❗ VERY RISKY — Gaps or rot
- Missing when needed, or outdated/wrong/hard to find.
- **Cost later:** wasted time, bad choices, loss of trust.

---

## Choose by attributes (apply holistically)
- **Frequency:** frequent + repeatable → automate; rare + critical → small, in-flow cue or short checklist.
- **Variability:** stable → encode in types/scripts; fast-changing → keep guidance tiny and local.
- **Ambiguity:** if people guess wrong, add one line that removes guesswork.
- **Impact:** high-cost mistakes → fail fast with the fix; low-cost → rely on clearer naming/structure.
- **Source of truth:** keep facts in code, schemas, or scripts; don’t duplicate them in prose.
- **Lifespan:** long-lived intent → encode it; short-lived tips → keep them near the point of use.

---

## Simple rules
- Make code and names carry **what**; let small cues/checklists cover **next step**.
- Prefer executable truth (types, schemas, scripts) over prose you must babysit.
- Keep anything written **short, local, and versioned** with the thing it explains.
- Delete or regenerate when the source changes.



# On development primitives

- **Commit messages**: although relatively permanent, don't self-surface (especially when squashed), and not accessible to non-engineers. Don't over rely.
- **Unit tests**: Much more worth if done with T.D.D, but T.D.D depends on clear requirements. It is still worth writing tests after the fact.
