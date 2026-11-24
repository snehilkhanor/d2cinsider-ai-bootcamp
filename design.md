# Design guide for dashboards and pages

Any teammate that builds something visual, such as the Growth Analyst's dashboard, follows this file. It keeps everything your team produces looking like it came from one place.

To make it yours, change the colours below to your brand's and keep everything else.

## Mood

Calm and readable. A founder opens this on a Monday morning with a cup of tea. The one thing that needs attention should be impossible to miss, and nothing else should compete with it.

## Colours

| Role | Light | Dark |
|---|---|---|
| Page background | `#FAF6EF` | `#1C1712` |
| Card surface | `#FFFFFF` | `#27201A` |
| Text | `#2B2118` | `#F1E8DA` |
| Secondary text | `#7A6A5A` | `#A8998A` |
| Borders and dividers | `#E6DCCD` | `#3A3027` |
| Accent, for links and chart lines | `#A8541A` | `#E0934F` |
| Alarm | `#9B2C1F` on `#FBE9E4` | `#F08A78` on `#3A1F1A` |
| Good change | `#2F6B3A` | `#7CC48A` |
| Bad change | `#9B2C1F` | `#F08A78` |

Every page supports both light and dark, following the reader's device setting.

## Type

Use the fonts already on the device: `system-ui, -apple-system, "Segoe UI", sans-serif`. Do not load fonts from the internet. The page must open with no connection.

| Use | Size | Weight |
|---|---|---|
| Page title | 28px | Bold |
| Section label | 15px, uppercase, letter-spaced | Semibold, secondary colour |
| Headline sentence | 19px | Regular |
| Body and tables | 15 to 16px | Regular |
| Big numbers | 22 to 26px | Bold |
| Small notes | 13px | Regular, secondary colour |

## Layout

- One column, 980px at most, centred, 20px side padding. It must read well on a phone.
- Cards: card surface, 1px border, 8px corners, 16px padding. No shadows.
- Spacing: 12px between tiles, 36px above each section label.

## Components

- **Alarm card.** The most prominent block on the page. Alarm background, a 6px alarm-coloured bar on the left, the before and after numbers large, then the cause, then the action for this week.
- **Number tiles.** A grid that wraps. Each tile: label, value, change against last week with an up or down arrow, coloured by whether the change is good or bad for the business, not by direction.
- **Trend line.** One line, accent colour, four points, each labelled with its value. No gridlines.
- **Tables.** Left-aligned text, right-aligned numbers, a divider under each row. A missing value says "not available" in italic secondary text. Never a zero, never a guess.
- **Notes.** A bordered box in secondary text, for anything the reader should know about where the numbers came from.

## Rules

- Currency is `₹` with Indian grouping: ₹1,87,000.
- The page works when opened by double-click. All data is written into the file.
- No animation. No images. No icons beyond simple arrows.
- If a section has no data, leave the section out. Do not show an empty box.
