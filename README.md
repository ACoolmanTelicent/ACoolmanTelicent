- 👋 Hi, I’m @ACoolmanTelicent
- 👀 I’m interested in making pedestrian things automated, and valuable problems front and center
- 🌱 I’m currently learning about home labbing
- 💞️ I’m looking to collaborate on DX
- 📫 How to reach me is MS Teams

# On communication style

I'll try and be precise by default.

But if I can't think of anything better to do, I'll end up _biasing toward action_ BUT with some time, care and effort put aside for cleaning up any confusion I cause.

# On docs and code comments

Let’s prefer outcomes that remove the need for docs, then add only what helps in the moment.

---

## 🏆 BEST — No docs needed
- **Automate the task** so nobody needs to look anything up. See: [Toil (Google SRE)](https://sre.google/sre-book/toil/).
- **Make code speak for itself** (clear names, small functions). Comments should explain **why**, not **what**: [Google style — comments](https://google.github.io/styleguide/jsguide.html#js-comments).

---

## 👼 OK — Contextual help (a practical compromise)
- **Inline, just-in-time hints** that unblock the user where errors occur. See: [Contextual Help](https://www.nngroup.com/articles/contextual-help/) and [Error-Message Guidelines](https://www.nngroup.com/articles/error-message-guidelines/) (NN/g).
- **Example:** if `telicent-cli` stderr includes `network <sha> not found`, suggest `docker network prune`.
- **Evergreen intent comments**: short notes that link to rationale or policy when it prevents confusion.

---

## 📜 RISKY — Heavy/long-form docs
- **High maintenance**: one missed update and it’s stale.
- **Low uptake**: existence ≠ understanding. Organize by need with a clear model like [Diátaxis](https://diataxis.fr/) (tutorials, how-to, reference, explanation).

---

## ❗ VERY RISKY — Missing or misleading docs
- **Missing when needed** forces guesswork.
- **Outdated or wrong** actively misleads; sometimes **no doc is safer** than a bad one. Prefer automation or targeted, in-context help over big docs.

---

**Rule of thumb:** automate first; add small, contextual guidance where it saves time; keep long docs rare, accurate, and clearly structured.

# On development primitives

- **Commit messages**: although relatively permanent, don't self-surface (especially when squashed), and not accessible to non-engineers. Don't over rely.
- **Unit tests**: Much more worth if done with T.D.D, but T.D.D depends on clear requirements. It is still worth writing tests after the fact.
