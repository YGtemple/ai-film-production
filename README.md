<div align="right">

**[English](README.md)** · [简体中文](README.zh-CN.md)

</div>

# ai-film-production

Production methodology for an AI content channel — 44 knowledge shorts, plus one short film taken through an eight-stage pipeline.

<sub>~250 text artifacts · 48 finished films (6.79 GB, not included)</sub>

---

## What this is

"像素档案馆" is a channel of knowledge shorts, each explaining the engineering behind an everyday object:

> Why are manhole covers round · Why high-speed trains have no seatbelts · Why coins have ridged edges · Why the microwave door is really a wire mesh · Why bicycle wheels hang from their top spokes rather than resting on the bottom ones

8.5–9.6 minutes each, 1080p landscape, fully animated. 48 finished films.

What is archived here is the **production methodology** — not the films, but the documents that let 44 episodes be made to a consistent standard.

## Structure

```
01_账号策划/    47 files — per-episode publishing copy and account setup
02_选题脚本/   187 files — narration scripts, topic research, model reference
北平的雪/      203 files — one short film, complete pipeline artifacts
```

### 北平的雪 — an eight-stage pipeline, end to end

A separate project (not part of the shorts series) that ran the full eight-stage process:

| Stage | Artifact | Size |
|---|---|---|
| 00 research | `historical-research-v001.md` | 13.3 KB |
| 01 story | `synopsis-v001.md` | 5.7 KB |
| | `characters-v001.md` | 13.2 KB |
| | `treatment-v001.md` | 9.3 KB |
| 02 script | `screenplay-v001.md` | 15.5 KB |
| | `screenplay-timing-audit-v001.md` | 1.8 KB |
| 03 assets | `asset-registry-v001.md` | 4.0 KB |
| 04 prompts | `performance-master-v001.md` | 11.8 KB |

Every artifact carries a `-v001` suffix, matching the pipeline rule that each stage reads only the confirmed current version.

## Two documents worth reading closely

### synopsis-v001.md — story design in three layers

**Layer one, story.** Concrete: time, place, people, events.

**Layer two, metaphor.** Four images, each with a setup and a payoff:

| Image | Set up | Paid off |
|---|---|---|
| Snow | falls on felled tree stumps and half a steamed bun | thaws; water drips from the eaves; the child's breath carries laughter for the first time |
| The felled locust tree | the century-old tree at the alley mouth is cut to clear a firing line | a PLA soup kitchen stands beside the stump; new shoots after the snow |
| Half a steamed bun | pressed into the boy's hand as his father is taken | grain is distributed on entry; the bun becomes white flour and New Year dumplings |
| The Yongdingmen gate arch | the father is dragged out through its shadow | the army enters through the same arch, into the light |

The fourth is the one to study: the same spatial motif, first a dark passage, then a lit gate. The visual inversion was designed at concept stage, so the storyboard stage only has to execute it.

**Layer three, intent.** Five sub-layers: aesthetic, context, thesis, stance, and **habitual gestures**. The fifth lists three concrete actions (pushing his sister's hands into his sleeve, hunching at the sound of boots, rising on tiptoe to call out at the end), which gives the performance stage something executable instead of something to reinterpret.

### screenplay-timing-audit-v001.md — a timing table

| Scene | Budget | Dialogue chars | Estimate | Delta | Cause / handling |
|---|---|---|---|---|---|
| 1 Night abduction | 30 | 96 | 31 | +1 | dense dialogue, overlapping shouts; let the mother's cry run parallel to the dragging |
| 9 Fu Zuoyi's decision | 30 | 119 | 32 | +2 | all-dialogue scene; speed up or cut 4–6 characters from one speech |
| 12 Entry and reunion | 30 | 51 | 33 | +3 | equipment display eats time; cut across armour and cavalry in 2–3 shots |

Twelve scenes, 30 seconds each, 360 seconds total. The estimate came to 365 — a 1.4% delta, inside tolerance, so it was auto-filed. **The tolerance rule was fixed in advance** (5 seconds or 10%, whichever is larger), not invented afterwards.

The most useful column is the last one: **the fix was decided at estimate time**, not discovered during the edit.

## What transfers

1. **Design the payoff of every image at concept stage.** Otherwise a prop ends up unused and nobody notices until the cut.
2. **Write intent in five layers.** The fifth gives the performance stage executable instructions.
3. **Manage duration with an estimate table and a pre-agreed tolerance.**
4. **Version every artifact.** `-v001` plus a read-only-current-version rule removes ambiguity after several rounds.
5. **State delivery specs as numbers a tool can check.** 1920×1080, H.264 Baseline, yuv420p, AAC-LC 48 kHz.

## Note

Only text artifacts are included. Finished video (48 films, 6.79 GB), cover PNGs (74 files, 103 MB) and character art (203 files) are excluded on size.

This repository is an archive — the active copy lives in [ai-drama-master-suite](https://github.com/YGtemple/ai-drama-master-suite) under `cases/`.

## License

MIT
