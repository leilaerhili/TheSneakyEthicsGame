# The Sneaky Ethics Game

A role-driven ethics exercise dressed up as a strategy game. Three teams — Instagram, a university AI lab, and the US Government — make simultaneous yes/no decisions across three rounds about a psychological-profiling algorithm, offshoring compute to China, and how to handle a data breach. Civilians advocate but don't decide.

Players are told they're playing to win for their team. They're not told it's an ethics exercise until the debrief. The point is to get the tradeoffs to surface from incentives rather than from people performing ethics for an audience.

- [`game.pdf`](./game.pdf) — comprehensive gamemaster script


## Running it

Designed for ~12 players (3–4 per team plus civilians) and about 90 minutes. The script in `game.md` walks a Game Master through the world setup, three rounds with branching outcomes, the debrief, and a list of debrief questions.

## Compiling the PDF

```
pdflatex game.tex
```

Requires `tcolorbox` with the `skins` and `breakable` libraries (standard in TeX Live and MiKTeX).

## License

MIT — use it, run it, modify it. If you run a session and learn something interesting, I'd love to hear about it.
