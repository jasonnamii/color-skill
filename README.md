# color-skill

> 🇰🇷 [한국어 README](./README.ko.md)

**A bold two-tone HTML color system built from your palette screenshots — vivid paired color blocks, large rounded panels, and high-contrast typography on a dark stage.**

## Prerequisites

- **Claude Cowork or Claude Code** environment

## Goal

Most generated HTML pages default to safe, washed-out palettes. This skill does the opposite: it builds a striking first impression from strong complementary contrast and large color blocks. Each panel locks its background and text colors into a tight 1:1 pairing on a near-black stage, producing an Instagram-palette-card rhythm.

## When & How to Use

Triggers when you say `컬러 스킬`, `color-skill`, `this color pattern`, `컬러 패턴`, `팔레트 HTML`, or ask for an HTML page/site/report with vivid paired color blocks, rounded panels, high-contrast type, or strong complementary color rhythm. Hand it a palette screenshot or describe the colors and it generates the page.

## Use Cases

| Scenario | Prompt | What Happens |
|---|---|---|
| Palette → page | `"이 팔레트로 HTML 만들어줘"` | Builds a dark-stage page with paired color panels |
| Report styling | `"컬러 스킬로 리포트 꾸며줘"` | Applies high-contrast block rhythm to the content |
| Palette cards | `"인스타 팔레트 카드 스타일로"` | Generates Instagram-style palette cards |

## Key Features

- **Black stage base** — page background starts at `#000000`/`#050505`/`#07090b`
- **1:1 color pairing** — each panel's background and text are matched as a complementary pair
- **Large rounded panels** — bold blocks with high-contrast typography
- **Palette-screenshot driven** — extracts and applies colors from your reference image

## Installation

```bash
git clone https://github.com/jasonnamii/color-skill.git ~/.claude/skills/color-skill
```

## Update

```bash
cd ~/.claude/skills/color-skill && git pull
```

Skills placed in `~/.claude/skills/` are automatically available in Claude Code and Cowork sessions.

## Part of Cowork Skills

One of 25+ custom skills. See the full catalog: [github.com/jasonnamii/cowork-skills](https://github.com/jasonnamii/cowork-skills)

## License

MIT License — feel free to use, modify, and share.
