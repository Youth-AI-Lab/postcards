# Youth Ai Lab — Postcards

Vintage-style postcards summarising what each Youth Ai Lab partner has been running on the ground. Each card opens to a foldable accordion of workshop fiches with a single mood, a triptych (activity, who, mood) and one best practice focused on the youth.

Production URL: <https://youth-ai-lab.github.io/postcards/>

## Structure

```
postcards/
├── README.md
├── index.html                       Global postcards landing
├── france/
│   ├── index.html                   Pacman's landing
│   └── pacmans-postcard-01/         The folded postcard
│       ├── index.html
│       ├── hero.webp                Cover photo
│       ├── logo.png                 L.A.B. logo (lab home)
│       ├── step-XX(-b/-c).{png,jpg,jpeg}   3 photos per workshop
│       └── texts.md                 All copy for re-editing
├── italy/
│   ├── index.html                   FARO landing
│   └── faro-postcard-01/
│       ├── index.html
│       ├── hero.png
│       ├── logo.png                 Perlatecnica logo
│       └── …
└── template/
    └── index.html                   Original verso-flip template
```

## URL convention

- `/` — global postcards landing
- `/{country}/` — country landing (FARO, Pacman's, …)
- `/{country}/{team-slug}-postcard-{NN}/` — a single postcard

Country slugs: `france`, `italy`, `spain`, `belgium`.
Team slugs: `pacmans`, `faro`, `uab`, `digitale-wolven`.

## Conventions

- **Cover photo** is rendered black-and-white with a light sepia warmth (`grayscale(1) sepia(0.15) contrast(0.95) brightness(1.08)`) inside a colored two-line YAL frame.
- **Workshop photos** sit in a stack of 1 large + 2 thumbnails, with the colored border in the fiche's accent color.
- **Triptych** in each fiche fills the right column: Activity (30%) · Who (20%) · Mood (50%).
- **Best practice** is always framed around the youth at that age range, not the technology.
- **Dates** in the past timeline show month + year only; dates in the future timeline show full DD/MM/YYYY when the dates are confirmed.

## Shared assets

The lab logos and the YAL banner live in `Youth-AI-Lab/success-stories/CommonVisuals/`. The `template/` folder references them via `../../SuccessStories/CommonVisuals/`. The published postcards (`france/pacmans-postcard-01`, `italy/faro-postcard-01`) ship their own local copies.

## Local preview

```bash
cd /path/to/YouthAiLab        # parent of Postcards/ and SuccessStories/
python3 -m http.server 8765
# open http://localhost:8765/Postcards/
```

## Editing copy

Each published postcard has a `texts.md` file alongside `index.html`. Edit that file, then port the changes into `index.html` (no automatic build step).

## Co-funding

Co-funded by the European Union. Views and opinions expressed are however those of the author(s) only and do not necessarily reflect those of the European Union or the European Education and Culture Executive Agency (EACEA). Neither the European Union nor EACEA can be held responsible for them.
