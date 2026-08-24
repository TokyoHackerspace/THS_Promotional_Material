50mm Square Sticker
======================

Design concept, color variations, and print order records for the 50mm x 50mm square sticker.

> Note: If a fact is not confirmed, it is marked as **TBD**. Please do not fill these in by guessing.

---

## 1. Color Concept

**The color changes with every print run.** This is intentional. It makes the stickers collectible, and it gives members a reason to pick up a new one each time.

A few points follow from this.

- There is no "official" sticker color. No single color needs to be kept in stock forever.
- Choosing a color is not a decision that needs long discussion. Any color that works with the design is a valid choice.
- Reprinting a past color is acceptable, for example when a batch was small and ran out quickly. But a new color is the default.
- Many colors have not been used yet. There is plenty of room left.

The only real constraint is the one in section 5: the background must be dark enough for the white logo to stay readable.

---

## 2. Common Specification

| Item | Value |
|---|---|
| Finished size | 50mm x 50mm (square) |
| Design | Logo (tokyo hackerspace + Tokyo Tower motif) and URL |
| Logo | **White knockout by default** |
| Print process | CMYK |
| Master files | `.ai` and `.svg` in this directory |
| Preview | `.png` in this directory |
| Print order records | `orders/<year-month>/` |

### Exception to the white knockout rule

If the background color is too light, white knockout does not work. In that case a black logo is used. So far this applies to `black on white` and `black on yellow` (concept only, never printed).

---

## 3. Color Variations

A list of the color designs that exist. This is separate from the print records, because the same color can be printed more than once.

| Color | File | Background CMYK | RGB | Contrast (white) | Created | Printed |
|---|---|---|---|---|---|---|
| black on yellow | — | TBD | TBD | — | TBD | Never (concept only) |
| black on white | — | 0 / 0 / 0 / 0 | `#FFFFFF` | — | TBD | Yes, date TBD |
| white on light blue | `5050_blue` | 100 / 0 / 0 / 0 | `#00AEEF` | 2.5:1 | TBD | Yes, date TBD |
| white on orange | `5050_orange` | 0 / 35 / 85 / 0 | `#FBB03F` | 1.8:1 | TBD | TBD |
| white on black | `5050_black` | 0 / 0 / 0 / 100 | `#221E1F` | 19:1 | TBD | TBD |
| white on green | `5050_green` | 90 / 30 / 95 / 30 | `#006737` | 7.0:1 | TBD | Yes, around 2024 |
| white on red | `5050_red` | 0 / 100 / 100 / 0 | `#ED1B23` | 4.4:1 | TBD | Yes, 2025-12 |
| white on vivid orange | `5050_vivid-orange` | 0 / 70 / 100 / 0 | `#F15A22` | 3.3:1 | 2026-08 | 2026-08 |
| white on magenta | `5050_magenta` | 0 / 100 / 0 / 0 | `#EC008C` | 4.3:1 | 2026-08 | 2026-08 |
| white on navy | `5050_navy` | 100 / 85 / 0 / 10 | `#2E3192` | 10.7:1 | 2026-08 | 2026-08 |
| white on violet | `5050_violet` | 75 / 95 / 0 / 0 | `#662D91` | 8.9:1 | 2026-08 | Not yet |

"Contrast (white)" is the luminance contrast ratio between the background color and white. See section 5 for why this matters.

### Considered but not adopted

| Color | Background CMYK | RGB | Reason |
|---|---|---|---|
| white on teal | 60 / 0 / 20 / 20 | `#42929D` | Proposed by a member. The hue is only 9 degrees away from the existing light blue, so the two are hard to tell apart when placed side by side. On hold. If we adopt it, a darker version such as C85 / M0 / Y35 / K25 would separate better. |

### Colors not used yet

Yellow, brown, gray, lime, and deeper shades of most hues are still open.
Any of these is fine as long as the contrast guideline in section 5 is met.

---

## 4. Print Orders

Newest first. Full details are in each order directory.

### 2026-08 — Sticker Japan

See [`orders/2026-08/README.md`](orders/2026-08/) for the full record.

- Colors: vivid orange, magenta, navy
- Quantity: 500 per design (1,500 total)
- Material: art paper, gloss coating, square trim

**Why these three colors**

All previous stock was gone, so this lot was effectively a restart.

- Vivid orange and magenta are new colors, so they cannot be confused with older stock.
- Navy is also new, and it is dark enough to work as the "safe" color that suits any laptop or case.
- The hues are spread across the color wheel (25° / 324° / 239°), so the three designs look clearly different when placed together.

Violet was designed at the same time but not printed in this lot.

**Result and notes**

TBD. Please record at least the following.

- How the printed color compares to the CMYK values on screen
- Whether the URL line (thin, small white text) is readable, especially on vivid orange
- Whether the black or navy solid areas look uneven
- How fast each color runs out. This tells us whether 500 per design is the right quantity next time
- Photos of the finished stickers

---

## 5. Design Notes

Lessons that stay useful for future lots.

### White knockout needs enough contrast

If the background is too light, the logo may still be readable but **the URL line disappears into the background**.

- As a rule of thumb, avoid backgrounds below 3:1 for white knockout.
- `#FBB03F` (1.8:1) fails this. To make orange work with a white logo, lower the brightness rather than raising the saturation. This is why `#F15A22` was used in 2026-08.
- `#00AEEF` (2.5:1) is also below the guideline, but it is kept as an established brand color.

### Fewer ink plates give a sharper knockout

The fewer inks a color uses, the less misregistration shows as a colored fringe around the white logo.

| Plates | Colors | Note |
|---|---|---|
| 1 | light blue (C), magenta (M), black (K) | Best |
| 2 | vivid orange (M+Y), violet (C+M) | Good. On orange, a small shift is hard to see because both inks are warm |
| 3 | navy (C+M+K) | Slightly worse |
| 4 | green (C+M+Y+K) | Worst. A colored fringe can show on the URL line |

### Solid black

- With **digital printing**, K100 is fine. No uneven areas, no registration problems.
- With **offset**, a large K100 area looks uneven. Adding C30-40 is the usual fix, but then a shift in the C plate can show as a blue fringe on the thin white text.
- Small sticker runs are almost always digital, so K100 is usually the simplest choice. Confirm with the vendor.

### Number of colors does not drive cost

CMYK process printing has no per-color plate charge. Adding another color costs almost nothing. There is no need to cut the number of colors to save money.
This makes the rotating color concept cheap to keep going, and it also means a variety pack costs about the same as a single color.

---

## 6. Open Items

- [ ] CMYK values for `black on yellow` — check if the original concept files still exist
- [ ] Order date, vendor, and quantity for the older lots
- [ ] Whether `white on orange` (`#FBB03F`) and `white on black` were ever actually printed
- [ ] Creation dates for the older color designs
- [ ] What to do with the teal proposal (`#42929D`)
- [ ] Art paper is an indoor material. Consider PVC or PET next time if the stickers need to survive rain and rubbing
