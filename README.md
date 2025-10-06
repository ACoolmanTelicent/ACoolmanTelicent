- 👋 Hi, I’m @ACoolmanTelicent
- 👀 I’m interested in making pedestrian things automated, and valuable problems front and center
- 🌱 I’m currently learning about Telicent
- 💞️ I’m looking to collaborate on ___
- 📫 How to reach me probably Frontend team "wall"

# On communication style

I'll try and be precise by default.

But if I can't think of anything better to do, I'll end up _biasing toward action_ BUT with some time, care and effort put aside for cleaning up any confusion I cause.

# On docs and code-comments

We shouldn't be patting ourselves on the back for creating documentation

1. 🏆 **BEST** No need for docs
    - A process might be automated
    - Code might be self-explanatory
2. 👼 **OK** Contextual docs/help = Compromised
      - The process/idea largely anticipatable itself, but relevant plugs any gaps
      - **Example**: IF telicent-cli stderr includes "network <sha> not found>" THEN display "Try 'docker network prune'"
  - **Example**: The code links to outside intentions - an ever-green comment about intention could be a cheap/quick solution
3. 📜 **RISKY**  Detailed accurate Documentation = One missed update cycle away from #5
      - Just because docs exist, does not mean they will read and interpreted as the writer intended.
4. **VERY RISKY** 
    - No docs when they are needed OR,
    - Inaccurate/degraded/unfindable docs = One missed update cycle away from #3 (No information is better than mis-information)

# On development primitives

- **Commit messages**: although relatively permanent, don't self-surface (especially when squashed), and not accessible to non-engineers. Don't over rely.
- **Unit tests**: Much more worth if done with T.D.D, but T.D.D depends on clear requirements. It is still worth writing tests after the fact.
