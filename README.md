# BWA-InputTilt

Broad spectral pre-shaping with 24-band overlay + A/B reference + LUFS-match.

**Category C** · **Tier 3** · part of the
[Bandwidth Audio](https://github.com/vmcguire) plugin ecosystem.

---

## What this is

BWA-InputTilt applies a 1st-order spectral shelf before band splitting — useful for taming bright sources or warming up dull ones at the input stage.

24-band visualization overlays the tilt curve on the live spectrum. A/B button with LUFS-match (no level cheating). Multi-anchor tilt (not just full-spectrum slope). GROUP scope: same tilt curve across all drum tracks before split.

For the broader story of *what BWA is building and why*, see
[BWA-Architecture](https://github.com/vmcguire/BWA-Architecture) —
specifically:

- [`USER-STORY-MAP.md`](https://github.com/vmcguire/BWA-Architecture/blob/main/docs/USER-STORY-MAP.md)
  — where this plugin sits in the bedroom-producer journey (Stage 7 — MIX).
- [`ECOSYSTEM.md`](https://github.com/vmcguire/BWA-Architecture/blob/main/ECOSYSTEM.md)
  — the full product map and the dual-surface / single-DSP architecture.
- [`docs/MARKET-PAIN-AND-ATTACKS.md`](https://github.com/vmcguire/BWA-Architecture/blob/main/docs/MARKET-PAIN-AND-ATTACKS.md)
  — what this plugin attacks (the pain it solves) and how.

## How this fits with the rest of BWA

BWA-InputTilt ships on **two surfaces** — same DSP, different UI:

1. **Standalone VST3** — drops into any DAW like a FabFilter / iZotope plugin.
   That's what this repo releases.
2. **Embedded cell inside BWA-Mix** — appears as a per-band / per-group cell
   processor inside BWA-Mix's track grid, sharing BWA-Mix's already-running
   band split and contributing to ecosystem-level cross-plugin features.

Both surfaces consume the **same authoritative DSP module**. Fix a bug once,
fixed everywhere.

## Status

🔴 Not built. Stub repo. Build target: Phase D extended.

## Releases

Versioned `.vst3` builds for macOS land in this repo's
[Releases](https://github.com/vmcguire/BWA-InputTilt/releases). Build from
source if you want — see `CLAUDE.md` for the dev surface (it's not this repo).

## License

Proprietary. Distribution + license terms pending storefront launch — see
[BWA-Architecture/docs/GO-TO-MARKET.md](https://github.com/vmcguire/BWA-Architecture/blob/main/docs/GO-TO-MARKET.md).
