- 👋 Hi, I’m @ACoolmanTelicent
- 👀 I’m interested in making pedestrian things automated, and valuable problems front and center
- 🌱 I’m currently learning about Telicent
- 💞️ I’m looking to collaborate on ___
- 📫 How to reach me probably Frontend team "wall"

# On communication style

I'll try and be precise by default.

But if I can't think of anything better to do, I'll end up _biasing toward action_ BUT with some time, care and effort put aside for cleaning up any confusion I cause.

# On docs and code-comments

In the pantheon of holy knowledge transfer techniques:

**Higher in list is better; Lower number is worse**

1. 🏆 No need for docs = The Holygrail is no need for docs
    - A process might be automated
    - Code might be self-explanatory
2. 👼 Contextual docs/help = Compromised
  - The process/idea largely anticipatable itself, but relevant plugs any gaps
  - **Example**: IF telicent-cli stderr includes "network <sha> not found>" THEN display "Try 'docker network prune'"
  - **Example**: The code links to outside intentions - an ever-green comment about intention could be a cheap/quick solution
3. 📜 Detailed accurate Documentation = One missed update cycle away from #5
  - Just because docs exist, does not mean they will read and interpreted as the writer intended.
4. 📜 No docs
  - No information is better than mis-information
5. 📜 Inaccurate/degraded docs = One missed update cycle away from #3
  - No information is better than mis-information

Then each of these techniques can have holy attributes. For instance:
- conventional/idiomatic: lessen the need for docs, and make editing automation easier). 
- discoverable: docs/help/automation scripts that are easily found are better than those that are hard to find
 
And of course unholy attributes - e.g. dependencies that are not enforced - like test failures that don't block PR

We shouldn't be patting ourselves on the back for creating documentation, we should be celebrating how/when our teammates achieve outcomes

Idle thought: I'd really love a file watched on yarn.lock that give me a big notification saying "Yo, you just changed yarn.lock"

# On development primitives

- **Commit messages**: although relatively permanent, don't self-surface (especially when squashed), and not accessible to non-engineers. Don't over rely.
- **Unit tests**: Much more worth if done with T.D.D, but T.D.D depends on clear requirements. It is still worth writing tests after the fact.
