---
marp: true
theme: default
paginate: true
header: "**MARP Cheatsheet** · Theme Reference · 2026"
footer: "Your footer (it can be anything)"


---
<style>
@import "styles/iee_style.css";
</style>
<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 1 — TITLE                                      -->
<!-- ══════════════════════════════════════════════════════ -->
<!-- _class: lead -->
<!-- _backgroundColor: #0f172a -->
<!-- _color: #f1f5f9 -->
<!-- _paginate: false -->
<!-- _header: "" -->
<!-- _footer: "" -->

<span style="font-family:'Syne',sans-serif;font-size:0.72em;color:#6366f1;letter-spacing:.15em;text-transform:uppercase;font-weight:700;">Complete Reference · 2026</span>

# MARP Theme
# Cheatsheet

### Everything you need to build slides with *this theme*

<br>

<span style="font-size:0.75em;color:#64748b;">Layouts · Images · Text · Components · Logos · Code · Tables</span>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 2 — TABLE OF CONTENTS                          -->
<!-- ══════════════════════════════════════════════════════ -->

## What's Inside

<div class="columns" style="margin-top:20px;">
<div>

**Slide Structure**
- Front matter & global config
- Slide separators (`---`)
- Per-slide directives (`<!-- -->`)
- Scoped styles

**Text & Typography**
- Headings H1 → H3
- Bold, italic, inline code
- Bullet lists & numbered lists
- Blockquotes

</div>
<div>

**Images**
- Background image: left / right / top / full
- Dual split backgrounds
- Inline `<img>` with sizing
- Logo placement (header, corner, watermark)

**Components (HTML)**
- `.columns` 2-col grid
- `.columns-3` 3-col grid
- `.card` panels
- `.highlight-box` gradient panels
- `.tag` badges
- Tables · Code blocks · Mermaid

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 3 — FRONT MATTER REFERENCE                     -->
<!-- ══════════════════════════════════════════════════════ -->

## Front Matter — Global Config

The YAML block at the very top (before the first `---`) controls the whole deck.

```yaml
---
marp: true                        # enables MARP
theme: default                    # base theme (default | gaia | uncover)
paginate: true                    # show page numbers
header: "**My Deck** · 2026"      # appears top-left every slide (markdown OK)
footer: "© My Lab"                # appears bottom-left every slide
style: |                          # inject global CSS (indent with 2 spaces)
  section { font-size: 22px; }
---
```

<div class="columns" style="margin-top:18px;">
<div class="card">

### Header / Footer tips

- Supports **bold**, _italic_, `code`
- Add logo: `'![h:28](logo.png) My Lab'`
- Hide on one slide: `<!-- _header: "" -->`

</div>
<div class="card">

### Theme choices

| Value | Look |
|-------|------|
| `default` | light, minimal |
| `gaia` | colorful, opinionated |
| `uncover` | clean, centered |

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 4 — SLIDE DIRECTIVES                           -->
<!-- ══════════════════════════════════════════════════════ -->

## Per-Slide Directives

HTML comments at the top of a slide override settings *for that slide only*.  
Prefix with `_` to scope to one slide; without `_` it persists to all following slides.

```markdown
<!-- _class: lead -->              ← centered layout (title slides)
<!-- _backgroundColor: #0f172a --> ← custom bg colour
<!-- _color: #ffffff -->           ← override all text colour
<!-- _paginate: false -->          ← hide page number
<!-- _header: "" -->               ← hide header
<!-- _footer: "" -->               ← hide footer
```

<div class="highlight-box" style="margin-top:18px;">
<h3>⚡ One-slide vs persistent</h3>
<p><code style="background:rgba(255,255,255,0.15);color:white;"><!-- _class: lead --></code> affects <strong style="color:white;">this slide only</strong>.<br>
<code style="background:rgba(255,255,255,0.15);color:white;"><!-- class: lead --></code> (no underscore) affects <strong style="color:white;">this slide AND all following</strong>.</p>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 5 — SCOPED STYLES                              -->
<!-- ══════════════════════════════════════════════════════ -->

## Scoped Styles — Per-Slide CSS

Use `<style scoped>` inside a slide to override CSS **only for that slide**.

<div class="columns" style="margin-top:16px;">
<div>

<div class="syntax">
&lt;style scoped&gt;<br>
&nbsp;&nbsp;section { background: #fdf4ff; }<br>
&nbsp;&nbsp;h2 { color: #9333ea; }<br>
&nbsp;&nbsp;ul li { font-size: 1.1em; }<br>
&lt;/style&gt;<br>
<br>
## This slide has purple h2<br>
<br>
- and a lavender background<br>
- without affecting other slides
</div>

</div>
<div class="card">

### When to use it

- One-off accent colours
- Special font sizes for dense slides
- Custom layout just for one slide
- Override global `.card` or `.columns` width
  
### Tip

Combine with `<!-- _backgroundColor -->` for full per-slide branding — useful for section dividers.

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 6 — TYPOGRAPHY                                 -->
<!-- ══════════════════════════════════════════════════════ -->

## Typography Reference

<div class="columns" style="margin-top:16px;">
<div>

<div class="syntax">
# H1 — Big title (Syne 800)<br>
## H2 — Section header (accented)<br>
### H3 — Subtitle / label (muted)<br>
<br>
Normal body text — DM Sans 400<br>
**Bold text** → renders in accent color<br>
*Italic/em text* → renders in amber<br>
`inline code` → dark chip<br>
<br>
&gt; Blockquote — indigo left border,<br>
&gt; light blue background
</div>

</div>
<div>

# H1
## H2
### H3

Normal body text — DM Sans 400

**Bold = accent color**  *Em = amber*

`inline code`

> Blockquote — indigo left border, light blue background

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 7 — LISTS                                      -->
<!-- ══════════════════════════════════════════════════════ -->

## Lists — Bullet, Numbered & Nested

<div class="columns" style="margin-top:16px;">
<div>

<div class="syntax">
Unordered list:<br>
- First item<br>
- Second item<br>
&nbsp;&nbsp;- Nested item<br>
&nbsp;&nbsp;- Another nested<br>
- Third item<br>
<br>
Ordered list:<br>
1. Step one<br>
2. Step two<br>
3. Step three<br>
<br>
Mixed:<br>
1. Main step<br>
&nbsp;&nbsp;- sub-detail<br>
&nbsp;&nbsp;- sub-detail
</div>

</div>
<div>

Unordered list:
- First item
- Second item
  - Nested item
  - Another nested
- Third item

Ordered list:
1. Step one
2. Step two
3. Step three

Mixed:
1. Main step
   - sub-detail
   - sub-detail

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 8 — IMAGES: BACKGROUND LEFT                    -->
<!-- ══════════════════════════════════════════════════════ -->

![bg left:42%](https://images.unsplash.com/photo-1677442135703-1787eea5ce01?w=900&q=80)

## `![bg left:XX%]`

Places the image on the **left**, text fills the right.

```markdown
![bg left:42%](images/photo.jpg)

## My Title

Content here flows to the right side.
```

**Rules:**
- `left:42%` → image takes 42% of slide width
- Recommended: **35–50%** for readable text
- Works with local files or URLs
- The `%` is optional — `![bg left]` defaults to 50%

<br>

> Tip: put the `![bg]` directive on the **first line** of the slide, right after `---`.

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 9 — IMAGES: BACKGROUND RIGHT                   -->
<!-- ══════════════════════════════════════════════════════ -->

![bg right:40%](https://images.unsplash.com/photo-1620712943543-bcc4688e7485?w=900&q=80)

## `![bg right:XX%]`

Places the image on the **right**, text fills the left.

```markdown
![bg right:40%](images/photo.jpg)

## My Title

Content here flows to the left side.
```

**Sizing modifiers** you can chain:

`![bg right:40% fit](img.png)` — contain inside box  
`![bg right:40% cover](img.png)` — crop to fill (default)  
`![bg right:40% auto](img.png)` — original size  

<br>

Works great for: portraits, product shots, charts you want to show alongside text.

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 10 — IMAGES: BACKGROUND TOP                    -->
<!-- ══════════════════════════════════════════════════════ -->

![bg top:48%](https://images.unsplash.com/photo-1639762681485-074b7f938ba0?w=1400&q=80)

<br><br><br><br><br>

## `![bg top:XX%]`

Image occupies the **top portion** of the slide, content sits below.

```markdown
![bg top:48%](images/photo.jpg)

<br><br><br><br><br>   ← push content below the image

## Title below the image
```

> Use `<br>` tags to push your text below the image area. The number of `<br>` needed depends on the percentage chosen.

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 11 — IMAGES: FULL BACKGROUND + OVERLAY         -->
<!-- ══════════════════════════════════════════════════════ -->

![bg](https://images.unsplash.com/photo-1451187580459-43490279c0fa?w=1600&q=80)

<!-- _header: "" -->
<!-- _footer: "" -->
<!-- _color: #ffffff -->

<div style="background:rgba(15,23,42,0.72);border-radius:16px;padding:32px 48px;backdrop-filter:blur(4px);">

## `![bg]` — Full Background Image

No percentage = image fills the **entire slide**.  
Add a semi-transparent overlay div to keep text readable.

```markdown
![bg](images/photo.jpg)
<!-- _color: #ffffff -->

<div style="background:rgba(15,23,42,0.72);
            border-radius:16px; padding:32px 48px;">

## Your Title

Your content here — readable on any image.

</div>
```

</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 12 — IMAGES: DUAL SPLIT BACKGROUND             -->
<!-- ══════════════════════════════════════════════════════ -->

![bg left:50%](https://images.unsplash.com/photo-1655720828018-edd2daec9349?w=800&q=80)
![bg right:50%](https://images.unsplash.com/photo-1620712943543-bcc4688e7485?w=800&q=80)

<!-- _color: #ffffff -->
<!-- _header: "" -->
<!-- _footer: "" -->

<div style="position:absolute;bottom:52px;left:50%;transform:translateX(-50%);background:rgba(15,23,42,0.85);border-radius:12px;padding:18px 36px;text-align:center;min-width:340px;">

## Two Images Side by Side

```markdown
![bg left:50%](left.jpg)
![bg right:50%](right.jpg)
```

Stack two `![bg]` directives — MARP splits them automatically.

</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 13 — IMAGES: INLINE SIZING                     -->
<!-- ══════════════════════════════════════════════════════ -->

## Inline Images — Size Control

MARP's native sizing syntax works on any inline `![]()` image.

<div class="columns" style="margin-top:16px;">
<div>

<div class="syntax">
Fixed width:<br>
![w:200](image.png)<br>
<br>
Fixed height:<br>
![h:120](image.png)<br>
<br>
Both (may distort):<br>
![w:200 h:120](image.png)<br>
<br>
Fit inside box:<br>
![w:200 h:120 fit](image.png)<br>
<br>
HTML for full control:<br>
&lt;img src="logo.png"<br>
&nbsp;&nbsp;&nbsp;style="width:180px;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;border-radius:8px;" /&gt;
</div>

</div>
<div class="card">

### When to use each

**`w:` / `h:`** — simple fixed size for icons and small illustrations.

**HTML `<img>`** — when you need `border-radius`, `box-shadow`, `object-fit`, `position:absolute`, or to place images inside a grid.

**`![bg]`** — always for background images. Never use `<img>` as a background — it won't fill the slide.

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 14 — LOGOS                                     -->
<!-- ══════════════════════════════════════════════════════ -->

## Logo Placement — 4 Techniques

<div class="columns-3" style="margin-top:20px;">

<div class="card">
<h3>① Header (every slide)</h3>

```yaml
header: '![h:30](logo.png) **Lab**'
```

Logo appears top-left on every slide. Hide on title slide with:

```markdown
<!-- _header: "" -->
```

</div>

<div class="card">
<h3>② Absolute corner</h3>

```html
<img src="logo.png"
  style="position:absolute;
         top:24px;
         right:48px;
         height:44px;" />
```

Paste inside any slide. Floats over all content.

</div>

<div class="card">
<h3>③ Watermark (CSS)</h3>

```css
section::after {
  content:'';
  background: url('logo.png')
    no-repeat bottom right;
  background-size: 90px;
  opacity: 0.12;
  position:absolute;
  inset:0;
}
```

Add to global `style:` block.

</div>

</div>

<div class="card" style="margin-top:16px; border-top-color: var(--color-accent2);">
<strong>④ Inline per-slide</strong> — just drop <code>![h:36](logo.png)</code> anywhere in the slide content. Best for title slides where you want the logo prominently placed.
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 15 — 2-COLUMN LAYOUT                           -->
<!-- ══════════════════════════════════════════════════════ -->

## `.columns` — 2-Column Grid

<div class="columns" style="margin-top:16px;">
<div>

<div class="syntax">
&lt;div class="columns"&gt;<br>
&lt;div&gt;<br>
<br>
Left column content —<br>
any markdown works here.<br>
<br>
- bullet lists<br>
- code blocks<br>
- images<br>
<br>
&lt;/div&gt;<br>
&lt;div&gt;<br>
<br>
Right column content.<br>
<br>
&lt;/div&gt;<br>
&lt;/div&gt;
</div>

</div>
<div class="card">

### Options

Adjust column ratio with inline style:

```html
<div class="columns"
  style="grid-template-columns: 2fr 1fr;">
```

Adjust gap:

```html
<div class="columns" style="gap: 48px;">
```

Center content vertically:

```html
<div class="columns"
  style="align-items: center;">
```

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 16 — 3-COLUMN LAYOUT                           -->
<!-- ══════════════════════════════════════════════════════ -->

## `.columns-3` — 3-Column Grid

```html
<div class="columns-3">
  <div class="card"> ... </div>
  <div class="card"> ... </div>
  <div class="card"> ... </div>
</div>
```

<div class="columns-3" style="margin-top:16px;">

<div class="card">
<h3>Column A</h3>

Any content goes here — text, lists, images, code.

</div>

<div class="card">
<h3>Column B</h3>

Cards stack naturally — each column is equal width by default.

</div>

<div class="card">
<h3>Column C</h3>

Nest a second row of `.columns-3` below for a 3×2 grid.

</div>

</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 17 — CARD & HIGHLIGHT-BOX                      -->
<!-- ══════════════════════════════════════════════════════ -->

## `.card` & `.highlight-box` Components

<div class="columns" style="margin-top:16px;">
<div>

<div class="syntax">
&lt;div class="card"&gt;<br>
&lt;h3&gt;Card Title&lt;/h3&gt;<br>
<br>
White background, rounded corners,<br>
indigo top border, subtle shadow.<br>
Works with any inner content.<br>
&lt;/div&gt;<br>
<br>
&lt;div class="highlight-box"&gt;<br>
&lt;h3&gt;Box Title&lt;/h3&gt;<br>
&lt;p&gt;Gradient indigo/violet bg,<br>
white text. Use for callouts,<br>
warnings, key takeaways.&lt;/p&gt;<br>
&lt;/div&gt;
</div>

</div>
<div>

<div class="card">
<h3>Card Title</h3>

White background, rounded corners, indigo top border, subtle shadow.

Works with any inner content.
</div>

<div class="highlight-box" style="margin-top:14px;">
<h3>Box Title</h3>
<p>Gradient indigo/violet bg, white text. Use for callouts, warnings, key takeaways.</p>
</div>

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 18 — TAG BADGES                                -->
<!-- ══════════════════════════════════════════════════════ -->

## `.tag` — Inline Badges

Use `<span class="tag">` to create status badges, labels, or category pills inline with text.

<div class="columns" style="margin-top:16px;">
<div>

<div class="syntax">
Feature <span class="tag">New</span> — default indigo<br>
<br>
&lt;span class="tag"&gt;New&lt;/span&gt;<br>
<br>
Custom colours:<br>
&lt;span class="tag"<br>
&nbsp;&nbsp;style="background:#22c55e"&gt;<br>
&nbsp;&nbsp;Done<br>
&lt;/span&gt;<br>
<br>
&lt;span class="tag"<br>
&nbsp;&nbsp;style="background:#f59e0b"&gt;<br>
&nbsp;&nbsp;WIP<br>
&lt;/span&gt;<br>
<br>
&lt;span class="tag"<br>
&nbsp;&nbsp;style="background:#ef4444"&gt;<br>
&nbsp;&nbsp;Urgent<br>
&lt;/span&gt;
</div>

</div>
<div class="card">

**Result:**

<br>

Feature <span class="tag">New</span> default indigo

<br>

Status chips:

<span class="tag" style="background:#22c55e;">Done</span>
<span class="tag" style="background:#f59e0b;">WIP</span>
<span class="tag" style="background:#ef4444;">Urgent</span>
<span class="tag" style="background:#64748b;">Archived</span>

<br>

Works inline with any text, heading, or list item.

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 19 — TABLES                                    -->
<!-- ══════════════════════════════════════════════════════ -->

## Tables

<div class="columns" style="margin-top:16px;">
<div>

<div class="syntax">
| Column A | Column B | Column C |<br>
|----------|----------|----------|<br>
| Cell 1   | Cell 2   | Cell 3   |<br>
| Cell 4   | Cell 5   | Cell 6   |<br>
| Cell 7   | Cell 8   | Cell 9   |<br>
<br>
Alignment:<br>
| Left | Center | Right |<br>
|:-----|:------:|------:|<br>
| aaa  |  bbb   |   ccc |
</div>

</div>
<div>

| Column A | Column B | Column C |
|----------|----------|----------|
| Cell 1   | Cell 2   | Cell 3   |
| Cell 4   | Cell 5   | Cell 6   |
| Cell 7   | Cell 8   | Cell 9   |

Alignment:

| Left | Center | Right |
|:-----|:------:|------:|
| aaa  |  bbb   |   ccc |

</div>
</div>

> Tip: keep tables **inside `.card`** or `.columns` divs to control their width and avoid them spanning the full slide awkwardly.

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 20 — CODE BLOCKS                               -->
<!-- ══════════════════════════════════════════════════════ -->

## Code Blocks

Fenced with triple backticks + language name for syntax highlighting.

<div class="columns" style="margin-top:14px;">
<div>

<div class="syntax">
```python<br>
def hello(name: str) -> str:<br>
&nbsp;&nbsp;&nbsp;&nbsp;return f"Hello, {name}!"<br>
```<br>
<br>
```json<br>
{ "key": "value", "n": 42 }<br>
```<br>
<br>
```bash<br>
marp deck.md --pdf<br>
```<br>
<br>
```plaintext<br>
No highlight — raw text block<br>
```
</div>

</div>
<div>

```python
def hello(name: str) -> str:
    return f"Hello, {name}!"
```

```json
{ "key": "value", "n": 42 }
```

```bash
marp deck.md --pdf
```

```plaintext
No highlight — raw text block
```

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 21 — MERMAID DIAGRAMS                          -->
<!-- ══════════════════════════════════════════════════════ -->

## Mermaid Diagrams

MARP renders Mermaid natively in HTML output. Use ` ```mermaid ``` ` fenced blocks.

<div class="columns" style="margin-top:14px;">
<div>

<div class="syntax">
```mermaid<br>
graph LR<br>
&nbsp;&nbsp;A[Input] --> B{Decision}<br>
&nbsp;&nbsp;B -->|Yes| C[Action A]<br>
&nbsp;&nbsp;B -->|No| D[Action B]<br>
&nbsp;&nbsp;C --> E[Output]<br>
&nbsp;&nbsp;D --> E<br>
```<br>
<br>
Other diagram types:<br>
sequenceDiagram<br>
classDiagram<br>
gantt<br>
pie<br>
erDiagram
</div>

</div>
<div class="card">

### Notes

- Works in `--html` output ✅
- PDF rendering requires `--allow-local-files` + Chrome
- Keep diagrams **simple** — complex graphs render small
- Use `graph LR` (left→right) for wide slides, `graph TD` (top↓down) for tall content
- Mermaid styles inherit from MARP's CSS — use `%%{init: ...}%%` for custom colours

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 22 — DARK THEME SLIDE                          -->
<!-- ══════════════════════════════════════════════════════ -->

<!-- _class: invert-dark -->
<!-- _backgroundColor: #0f172a -->

## Dark Theme Slides

To switch a single slide to dark mode, add both directives at the top:

```markdown
<!-- _class: invert-dark -->
<!-- _backgroundColor: #0f172a -->
```

The `invert-dark` class (defined in global CSS) overrides heading colours, blockquote colours, and text — so everything stays readable on dark backgrounds.

> Works perfectly for section dividers, quote slides, or dramatic conclusions.

**What's automatically re-coloured:**
- `h2` → indigo `#818cf8`
- `blockquote` → dark surface `#1e293b`
- Body text → light `#f1f5f9`

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 23 — RENDER COMMANDS                           -->
<!-- ══════════════════════════════════════════════════════ -->

## Rendering Your Deck

<div class="columns" style="margin-top:16px;">
<div>

```bash
# HTML — keeps animations, Mermaid, fonts
marp deck.md --html

# PDF — best for sharing & printing
marp deck.md --pdf

# PowerPoint — editable in LibreOffice/PPT
marp deck.md --pptx

# Watch mode — auto-rebuild on save
marp deck.md --watch --html

# Custom output path
marp deck.md --pdf -o ./output/deck.pdf

# Allow local images in PDF
marp deck.md --pdf --allow-local-files
```

</div>
<div class="card">

### Output format guide

| Format | Use case |
|--------|----------|
| `--html` | Browser presentation, Mermaid, animations |
| `--pdf` | Sharing, printing, archiving |
| `--pptx` | Client handoff, further editing |

### Image path tip

For **local images** in PDF export, always add `--allow-local-files`:

```bash
marp deck.md --pdf --allow-local-files
```

Without it, local `images/` paths are blocked by Chrome's security sandbox.

</div>
</div>

---

<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 24 — QUICK REFERENCE TABLE                     -->
<!-- ══════════════════════════════════════════════════════ -->

## Quick Reference

| Feature | Syntax |
|---------|--------|
| Slide separator | `---` on its own line |
| Title slide | `<!-- _class: lead -->` |
| Dark slide | `<!-- _class: invert-dark -->` + `<!-- _backgroundColor: #0f172a -->` |
| Hide header | `<!-- _header: "" -->` |
| Image — left | `![bg left:42%](img.png)` |
| Image — right | `![bg right:42%](img.png)` |
| Image — top | `![bg top:48%](img.png)` |
| Image — full | `![bg](img.png)` |
| Two images | `![bg left:50%](a.png)` + `![bg right:50%](b.png)` |
| Inline image size | `![w:200](img.png)` or `![h:80](img.png)` |
| Logo in header | `header: '![h:30](logo.png) My Title'` |
| 2-col layout | `<div class="columns"><div>…</div><div>…</div></div>` |
| 3-col layout | `<div class="columns-3">…</div>` |
| Card panel | `<div class="card">…</div>` |
| Gradient box | `<div class="highlight-box">…</div>` |
| Badge | `<span class="tag">Label</span>` |
| Mermaid | ` ```mermaid … ``` ` |
| Per-slide CSS | `<style scoped> … </style>` |

---
## References

<div class="references">
<p>[1] LeCun, Y., Bengio, Y., & Hinton, G. (2015). Deep learning. <em>Nature</em>, 521, 436–444. <a href="https://doi.org/10.1038/nature14539">doi:10.1038/nature14539</a></p>
<p>[2] Vaswani, A. et al. (2017). Attention is all you need. <em>Advances in Neural Information Processing Systems</em>, 30.</p>
<p>[3] Brown, T. et al. (2020). Language models are few-shot learners. <em>NeurIPS</em>.</p>
</div>

----


<!-- ══════════════════════════════════════════════════════ -->
<!--  SLIDE 25 — CONCLUSION                                -->
<!-- ══════════════════════════════════════════════════════ -->

<!-- _class: lead -->
<!-- _backgroundColor: #0f172a -->
<!-- _color: #f1f5f9 -->
<!-- _paginate: false -->
<!-- _header: "" -->
<!-- _footer: "" -->

<div style="text-align:center;">

<div style="font-size:2.6em;margin-bottom:8px;">📐</div>

# You're Ready to Build

<br>

<div style="max-width:580px;color:#94a3b8;font-size:0.85em;line-height:1.75;">
Copy the front matter block into any new <code style="background:#1e293b;color:#818cf8;">.md</code> file, separate slides with <code style="background:#1e293b;color:#818cf8;">---</code>, and use this cheatsheet as your reference for every layout, component, and image technique.
</div>

<br>

<div style="display:flex;gap:16px;justify-content:center;flex-wrap:wrap;">
  <div style="background:#1e293b;border-radius:10px;padding:10px 20px;font-family:'Syne',sans-serif;font-size:0.7em;color:#818cf8;">![bg left/right/top]</div>
  <div style="background:#1e293b;border-radius:10px;padding:10px 20px;font-family:'Syne',sans-serif;font-size:0.7em;color:#818cf8;">.columns / .card</div>
  <div style="background:#1e293b;border-radius:10px;padding:10px 20px;font-family:'Syne',sans-serif;font-size:0.7em;color:#818cf8;">.tag / .highlight-box</div>
  <div style="background:#1e293b;border-radius:10px;padding:10px 20px;font-family:'Syne',sans-serif;font-size:0.7em;color:#818cf8;">style scoped</div>
</div>

</div>