# HOP://MASTER-CONTROL

An engineering cockpit for **Hall of Paths** (the basketball life-sim at
https://visionary-lolly-3d978a.netlify.app/).

**▶ Use it here: https://coltstan.github.io/hop-master-control/**

The game's two pure-logic engines (`HOPEngine` + `HOPGM`, ~1,700 lines) are
extracted from the live build and embedded in a single HTML file, so every
number in this terminal comes from the game's REAL math — no game UI, no
saves touched, works fully offline. You can also just download
`index.html` (or `master-terminal.html`, same file) and double-click it.

## Stations

- **◉ OVERVIEW** — build telemetry (14,912 lines, ~1,050 functions, zero
  external deps), three-strata architecture map, analyst notes, and the
  localStorage registry.
- **▤ CODE MAP** — section-by-section index of the 15k-line source with
  line numbers, plus the live export surface of both engines (click any
  export to inspect it in the terminal).
- **▮ TERMINAL** — a REPL wired to the engine:
  `league` · `season` · `run <n>` · `draft` · `prospect [pos]` ·
  `name [n]` · `bloodline` · `legends` · `hall champ=4 mvp=2 …` ·
  `value <ovr> <age>` · `seed <n>` · `js <expr>` · `help` · `clear`
- **⚗ SIM LAB** — one-click Monte-Carlo experiments: 1,000-prospect talent
  distribution, develop-300-prospects-to-27 ceiling study, 20-season
  dynasty/parity sim, 500 bloodline variance rolls, draft-class audit.
- **♛ HALL LAB** — the exact Hall-of-Fame formula, live: type a résumé,
  see points, tier verdict, the peak-dominance gate, and where you slot
  among the 20 parody legends. Presets included (GOAT run, Ringless MVP,
  Compiler, One-year wonder).
- **⇄ TRADE LAB** — the GM engine's market brain per team: salaries vs
  fair cost, surplus trade value, scout reads, plus a scouting-fog demo
  showing six markets disagreeing about the same prospect's ceiling.
- **▦ DATA BANKS** — the content tables read live from the engine:
  legends, teams (with colors), hidden badges, the 5×20 bloodline grid,
  the parent pools, and the full legacy-scoring value tables.

## Notes

- Engine code © the Hall of Paths author; extracted here unmodified for
  introspection and tooling. The terminal UI layer is the only new code.
- Everything runs client-side. No network calls, no tracking, no saves.
