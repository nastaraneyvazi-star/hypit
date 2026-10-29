# Progress

- **Status:** v1 delivered — `deliverables/tech-founders-tier.mp4` (720×1280, 30 fps, 26.4 s, AAC audio).
- **Build:** `bld_20261029T002154885Z_C5762AF8B2` (`runs/final.svrun`, Profile `hypit.runtime.json`,
  local only, $0). Re-render: `hypit build runs/final.svrun --runtime ./hypit.runtime.json --follow`.
- **Source:** `authors/main.svml` (timeline, text, board), `recipes/look.svs` (colours, sizes),
  tiles in `assets/icons/` (generated locally from HTML), audio reused from the Hypit football example.
- **Known workarounds (Hypit 0.3.1):**
  - text-fine auto-generates the same run id (`run-1`) in every paragraph, so multi-paragraph
    Flows give each line an explicit `<typo:Span id>`.
  - the HTML text renderer allows line breaks between any two graphemes, so automatic wrapping
    splits words. Every multi-word line uses an explicit `<typo:Break/>`; keep new lines short enough to fit.
- **Possible next steps:** change founders, tiers or jokes (the table in TREATMENT.md mirrors the source);
  louder mix (music gain 0.22; peak −12 dB); real photos instead of initials tiles; an AI host/voice
  (paid, needs a HypiHub account or API keys and a new budget decision).
