# Digitale Wolven · A Belgian postcard from Digitale Wolven — Postcard text

All copy on the postcard, ready for rewriting.
Path: `Postcards/belgium/digitale-wolven-postcard-01/index.html`

Everything in square brackets is a slot to fill. Fill this file first, then port the
changes into `index.html` (no automatic build step).

---

## Page title (browser tab)

> Digitale Wolven · A Belgian postcard from Digitale Wolven

---

## Stamp / postmark

- Stamp avatar: wolf (emoji, stands for the Wolven; swap for a small SVG if the team prefers)
- Stamp logo: Digitale Wolven. Drop `logo.png` in the folder, then replace the `.s-name` block with the `.s-logo` image.
- Postmark: **[City]**, [DD/MM/YYYY]

---

## Cover (recto)

### Pills

- `Digitale Wolven · Belgium`
- `[Mon Year] → [Mon Year]`

### Headline

> From Digitale Wolven to the **Youth AI Lab** · [three-word promise].

### Subhead

> [Two or three sentences: how many workshops, over which months, the threads they followed, and who was in the room. Keep it concrete, no jargon.]

Hero photo: `hero.png` (missing for now; the cover carries the `no-photo` class, remove it once the photo is in the folder)

### Stats

| Number | Label |
|---|---|
| [N] | Sessions |
| [Nh] | In the lab |
| [N] | Researchers |

---

## Past timeline (visible when closed)

### Header

- Title: **Workshops done**
- Label: `[N] sessions at Digitale Wolven`

### Steps

1. **[Mon Year]** · [Workshop title].
2. **[Mon Year]** · [Workshop title].
3. **[Mon Year]** · [Workshop title].

To add a fourth step, set `.timeline-past { grid-template-columns: repeat(4, 1fr); }`.

---

## Unfold button

- Closed: `Unfold the journey ▸`
- Open: `Fold back ▸`

---

## Fiche 01 · [Mon Year] · accent pink

**Title:** [Workshop title] · [what it was about].

**What we ran:**
[Four to six sentences telling the session as it happened: how it opened, what the youth handled, what shifted, how it closed. Present the steps in order. No captions, no meta commentary.]

**Activity:**
- [Activity name]
- Ideation sheet: `https://github.com/Youth-AI-Lab/deliverables/raw/master/Ideation_Sheets/[SheetFileName].pdf`

**Who:**
- [Group name]
- [Age range] yo

**Mood:**
[Two adjectives, then one sentence on what the room actually felt like.]

**Skill tree:** [skill] · [skill] · [skill] · [skill]

**Best practice:**
[One or two sentences about the youth at that age, not about the technology or the logistics.]

**Pictures:** `step-01.png` · `step-01-b.png` · `step-01-c.png`

---

## Fiche 02 · [Mon Year] · accent blue

**Title:** [Workshop title] · [what it was about].

**What we ran:**
[Four to six sentences telling the session as it happened.]

**Activity:**
- [Activity name]
- Ideation sheet: `https://github.com/Youth-AI-Lab/deliverables/raw/master/Ideation_Sheets/[SheetFileName].pdf`

**Who:**
- [Group name]
- [Age range] yo

**Mood:**
[Two adjectives, then one sentence on what the room actually felt like.]

**Skill tree:** [skill] · [skill] · [skill] · [skill]

**Best practice:**
[One or two sentences about the youth at that age.]

**Pictures:** `step-02.png` · `step-02-b.png` · `step-02-c.png`

---

## Fiche 03 · [Mon Year] · accent orange

**Title:** [Workshop title] · [what it was about].

**What we ran:**
[Four to six sentences telling the session as it happened.]

**Activity:**
- [Activity name]
- Ideation sheet: `https://github.com/Youth-AI-Lab/deliverables/raw/master/Ideation_Sheets/[SheetFileName].pdf`

**Who:**
- [Group name]
- [Age range] yo

**Mood:**
[Two adjectives, then one sentence on what the room actually felt like.]

**Skill tree:** [skill] · [skill] · [skill] · [skill]

**Best practice:**
[One or two sentences about the youth at that age.]

**Pictures:** `step-03.png` · `step-03-b.png` · `step-03-c.png`

---

## Next investigations (visible when open)

### Header

- Title: **Next investigations**

### Dates (DD/MM/YYYY on the spots)

- [DD/MM/YYYY]
- [DD/MM/YYYY]
- [DD/MM/YYYY]
- [DD/MM/YYYY]
- [DD/MM/YYYY]
- [DD/MM/YYYY]

The last spot carries the `tomorrow` class (orange dot). For a different number of
spots, set `.timeline.timeline-many { grid-template-columns: repeat(N, 1fr); }`.

### Single subtext

[Two sentences: through which month the sessions run, which threads they continue, and that a detailed plan follows each session as it is delivered.]

---

## Editorial notes

- No em dashes (use `·` middle dots or commas/colons).
- No captions on photos.
- 3 fiches for now, each with: title, **What we ran** moment, Activity / Who / Mood triptych (30 / 20 / 50 %), Skill tree, Best practice. Add a fiche by copying a `.fiche` block and giving it the next accent in the rotation (pink, blue, orange, green, yellow).
- The Best practice is meant to be about **the youth at that age range**, not the tech or logistics.
- Targets a general public audience.
- Card colours: green and blue frame, yellow third line. Fiche accents rotate pink, blue, orange.
- All content describes what was done BEFORE the postmark date.
