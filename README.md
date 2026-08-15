# lizpratt.github.io

Portfolio site for Elizabeth Pratt, PhD. Jekyll, served by GitHub Pages.

## How to change things

| I want to... | Edit this |
| :--- | :--- |
| Change the home page | `index.html` |
| Change the about page | `about.md` |
| Edit a case study | `_work/ibm-concert.md` or `_work/ibm-network-intelligence.md` |
| Add a new case study | Copy an existing file in `_work/`, give it a new `index:` number |
| Change colors, type, spacing | `assets/css/main.css` (tokens live at the top) |
| Change nav, footer, name | `_layouts/default.html` |
| Change email / LinkedIn / site title | `_config.yml` |
| Add images | Drop them in `assets/img/` |

The design system is documented in `DESIGN.md`.

## Publishing

Commit and push to `main`. GitHub Pages rebuilds in about a minute.

## Building blocks inside a case study

Numbered section head:

    {% include chapter.html num="§ 03" title="Naming the job" %}

A figure:

    {% include fig.html num="04" src="/assets/img/nwi/jtbd_map.png"
       caption="The job map." source="Optional provenance line." %}

A before/after pair:

    {% include pair.html num="12" a_label="Before" a_src="/assets/img/x.png"
       b_label="After" b_src="/assets/img/y.png" caption="What changed." %}

A pull statement:

    <div class="statement reveal"><p>The sentence you want remembered.</p></div>
