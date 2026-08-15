# Design system: Ledger

The system behind lizpratt.github.io. Editorial, print-inspired, deliberately not a template.

## The idea

A research portfolio should look like something a researcher made: set with care, argued in prose,
carrying its evidence in figures. The reference points are academic journals, exhibition catalogues,
and well-made annual reports, not SaaS marketing pages.

Three rules do most of the work.

**Paper, not screen.** The canvas is warm off-white, the ink is warm near-black. Nothing is pure
#FFFFFF or #000000. The page should feel printed.

**Rules, not boxes.** Structure comes from hairline rules and whitespace. There are no cards, no
drop shadows, no rounded containers, no gradients. Corners are square.

**Two voices.** A high-contrast serif carries every human sentence. A mono carries every machine
label: section numbers, figure numbers, metadata, captions, dates. Nothing is set in a neutral
UI sans, because that is what makes a page look generated.

## Type

| Role | Family | Detail |
| :--- | :--- | :--- |
| Display and body | Newsreader (variable, optical sizing) | Weight 200 for display, 400 for prose, italic for emphasis |
| Labels and data | IBM Plex Mono | Uppercase, tracked +0.12em, small sizes only |

Newsreader is a contemporary transitional serif with real optical sizing, so display sizes get
tighter and finer while body sizes stay open. IBM Plex Mono is the nod to a decade at IBM and
gives the metadata a lab-notebook precision.

Scale (fluid, `clamp()`):

- `display` 46 to 84px, weight 200, line-height 1.02, letter-spacing -0.02em
- `title` 32 to 48px, weight 300, line-height 1.08
- `heading` 24 to 30px, weight 400, line-height 1.2
- `lede` 20 to 25px, weight 300, line-height 1.5
- `body` 18.5px, weight 400, line-height 1.65
- `meta` 12px mono, uppercase, tracked

Prose measure is capped at 34rem, roughly 66 characters. Nothing runs wider.

## Color

Light (default):

```
paper       #FAF7F2   warm off-white canvas
paper-deep  #F1ECE2   inset panels, figure mats
ink         #17150F   body text
ink-2       #514B40   secondary prose
ink-3       #6E6858   captions, metadata (WCAG AA, 5.2:1 on paper)
rule        #DED6C7   hairlines
spot        #B8431F   vermillion; the only color in the system
spot-deep   #8E3116   spot on hover
```

Dark:

```
paper       #141310
paper-deep  #1D1B16
ink         #EFEBE1
ink-2       #B8B1A3
ink-3       #877F70
rule        #33302A
spot        #E4744C
```

The spot is used sparingly: section numbers, the rule under a section number, link underlines on
hover, the "before/after" markers. If more than roughly two percent of the page is vermillion,
it is being overused.

## Layout

A 12-column grid on a 1240px max width with 3.5rem gutters. Three habitual placements:

- **Measure.** Prose sits in columns 3 through 9. Left-aligned, never centered.
- **Margin.** Section numbers and chapter numbers stack directly above the heading they label, in
  the same column — never beside it. A number sitting in its own column next to a heading is a
  templated pattern we deliberately avoid.
- **Full.** Figures may break out to the full 12 columns when the diagram earns it.

Vertical rhythm is a 8px base. Section breaks are 8rem on desktop, 4.5rem on mobile.

## Figures

Every figure gets a mono caption in three parts: a figure number in spot color, a description, and
where the artifact came from. Diagrams sit on `paper-deep` with a hairline border and generous
inset padding so the artwork never touches the frame. Screenshots sit flush with no mat, because
they carry their own chrome.

Before/after pairs stack on mobile and sit side by side above 900px, each labeled in mono.

## Motion

Almost none. Links transition their underline over 120ms. Figures fade in on scroll over 500ms with
a 12px rise, once, and the whole effect is disabled under `prefers-reduced-motion`. There are no
parallax effects, no scroll-jacking, no counters that tick up.

## What this system refuses

Hero gradients. Glassmorphism. Rounded cards in a three-up grid. Emoji as iconography. Centered
sans-serif headlines over a photo. Animated statistic counters. "Let's build something amazing
together." Purple-to-blue anything. Italic headings — headers are always roman; emphasis inside a
heading or a display-scale statement is carried by weight or the spot color, never `font-style:
italic`. Italic is reserved for emphasis inside running body prose.
