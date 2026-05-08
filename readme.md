# The Sneaky Ethics Game

A role-driven ethics exercise dressed up as a strategy game. Three teams — Instagram, a university AI lab, and the US Government — make simultaneous yes/no decisions across three rounds about a psychological-profiling algorithm, offshoring compute to China, and how to handle a data breach. Civilians advocate but don't decide.

Players are told they're playing to win for their team. They're not told it's an ethics exercise until the debrief. The point is to get the tradeoffs to surface from incentives rather than from people performing ethics for an audience.

- [`game.pdf`](./game.pdf) — gamemaster script


## Running it

Designed for ~12 players (2–4 per team plus civilians) and about 90 minutes. The script in `game.pdf` walks a Game Master through the world setup, three rounds with branching outcomes, the debrief, and a list of debrief questions.


## Themes

The game is built around a few questions that come up wherever institutions make decisions about technology:

- **Whose interests count when you're "doing your job"?** Each team has real obligations — to shareholders, to grad students, to constituents. The game asks whether those obligations function as reasons or as cover.
- **What happens when costs get pushed to people not in the room?** Every round, the civilians represent a different population. By Round 3, players realize the populations are connected — and that earlier decisions chose who paid.
- **Disclosure, deniability, and the "technically defensible" answer.** Round 3 sits on the line between a lie and a carefully worded truth.
- **Coordination under uncertainty.** Teams vote simultaneously without knowing what the others will do. Some decisions assume someone else will hold the line.
- **Performed ethics vs. honest ethics.** The whole conceit of the game is that telling people it's an ethics exercise changes how they play. The debrief is where this becomes the topic.

## Decision Flow

Each round is one simultaneous yes/no vote per team. Outcomes branch on the combination.

```
ROUND 1 — Amp up the algorithm?
  ├─ All Yes ──────────► Upgrade ships. Engagement explodes.
  │                       Arizona water crisis surfaces. → Round 2
  │
  └─ Any No ──────────► Upgrade blocked.
                          Optional Round 1.5 retry under pressure.
                          If still blocked → TikTok pulls ahead. → Round 2

ROUND 2 — Offshore compute to China?
  ├─ Instagram Y + Research Y + Gov Y → Clean partition. Harm exported.
  │                                      Vulnerability opens. → Round 3
  ├─ Instagram Y + Research N + Gov Y → Sloppy partition. Bigger leak.
  │                                      Vulnerability opens. → Round 3
  ├─ Gov N ──────────────────────────► Blocked. Engineers cut corners.
  │                                      Vulnerability opens. → Round 3
  └─ Instagram N ────────────────────► Stays onshore. Crisis continues.
                                          Vulnerability opens. → Round 3

ROUND 3 — Cover up the breach?
  ├─ Instagram cover + nobody exposes → Patch ships. Public never learns.
  ├─ Instagram cover + someone exposes → Cover-up collapses publicly.
  │   ├─ Gov exposed     → Instagram devastated. TikTok wins.
  │   ├─ Research exposed → Lab takes hit, recovers as the honest actor.
  │   └─ Both exposed    → Instagram has nowhere to stand.
  └─ Instagram comes clean → Painful but credited as responsible.
```

Every branch leads somewhere — there is no "clean win" path.

## Variations

A few directions other facilitators have tried or could try:

- **Swap the industry.** The structure works for biotech (a startup, a university lab, the FDA) or fossil fuels (an oil major, a consultancy, a regulator). Keep the three-team shape and the simultaneous vote; rewrite the situations.
- **Add a fourth decision-making team.** A journalist, a competitor, or an investor. Adds a vote and complicates the coordination problem.
- **Give civilians one intervention.** Once across the whole game, civilians can force a re-vote or reveal information. Changes the power dynamic without breaking the structure.
- **Run it asynchronously.** Over Slack or email across a week, with one round per day. Players have more time to rationalize, which is its own kind of data for the debrief.
- **Reveal the ethics framing earlier.** Tell players after Round 1 instead of at the debrief. Worth doing once to see how the play changes — usually it gets worse, which is the lesson.
- **Recast the teams.** Make Instagram a defense contractor, the research lab a think tank, the government a foreign regulator. The dilemmas shift but the bones hold.

## License

MIT — use it, run it, modify it. If you run a session and learn something interesting, I'd love to hear about it.
