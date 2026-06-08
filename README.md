# Fashionology Summit 2026 · Second Brain

Interactive single-file knowledge site for the Fashionology Summit 2026 deep report (NYC, June 6, 2026), built from verbatim transcripts of 14 on-site recordings + handwritten notes + the official agenda.

## Use

Open `index.html` directly in any browser — no server, no build step, works offline.

- **Left menu**: grouped, scrollable navigation (Start / 7 Panels / Insights) with per-module sub-sections and scroll-spy.
- **Search**: `⌘K` (or the search box) — full-text spotlight search across every panel; `↑↓` + `⏎` to jump.
- **Layer filter**: on panel pages, filter content by 主线 Key / 展开 Detail / 原话 Quotes.
- **Language**: 中 / EN toggle (full bilingual content).
- **Tables**: click any column header to sort (e.g. the Key Data module).
- **Mobile**: fully responsive; menu becomes a slide-over drawer, filters become a floating pill.

## Rebuild

Content lives in `content/*.md`. To regenerate `index.html` after editing:

```bash
pip install markdown
python3 build.py
```

`build.py` parses both markdown reports into structured JSON and injects it into `template.html`.

## Files

| File | Purpose |
|---|---|
| `index.html` | The site (self-contained, ~425 KB) |
| `content/Fashionology_Summit_2026_深度报告.md` | Chinese report (source of truth) |
| `content/Fashionology_Summit_2026_Deep_Report_EN.md` | English report |
| `build.py` + `template.html` | Build pipeline |
