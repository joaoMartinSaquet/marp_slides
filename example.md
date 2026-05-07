---
marp: true
theme: default
paginate: true
header: "**Agentic AI** · MCP & Claude · 2026"
footer: "© AI Research Lab — Slide production automation"
style: |
  @import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=DM+Sans:ital,wght@0,300;0,400;1,300&display=swap');

  :root {
    --color-primary:   #0f172a;
    --color-accent:    #6366f1;
    --color-accent2:   #f59e0b;
    --color-surface:   #f8fafc;
    --color-muted:     #64748b;
  }

  section {
    font-family: 'DM Sans', sans-serif;
    font-size: 22px;
    background: var(--color-surface);
    color: var(--color-primary);
    padding: 48px 60px;
  }

  h1, h2, h3 {
    font-family: 'Syne', sans-serif;
    font-weight: 800;
    letter-spacing: -0.02em;
  }

  h1 { font-size: 2.4em; color: var(--color-primary); }
  h2 { font-size: 1.7em; color: var(--color-accent); border-bottom: 3px solid var(--color-accent2); padding-bottom: 6px; display: inline-block; }
  h3 { font-size: 1.1em; color: var(--color-muted); font-weight: 600; }

  strong { color: var(--color-accent); }
  em { color: var(--color-accent2); font-style: normal; font-weight: 700; }

  code {
    background: #1e293b;
    color: #e2e8f0;
    border-radius: 4px;
    padding: 2px 6px;
    font-size: 0.85em;
  }

  pre {
    background: #0f172a;
    color: #e2e8f0;
    border-radius: 10px;
    padding: 24px;
    font-size: 0.75em;
    border-left: 4px solid var(--color-accent);
    box-shadow: 0 4px 24px rgba(0,0,0,0.15);
  }

  pre code { background: transparent; padding: 0; }

  table {
    width: 100%;
    border-collapse: collapse;
    font-size: 0.85em;
  }

  th {
    background: var(--color-accent);
    color: white;
    padding: 10px 14px;
    font-family: 'Syne', sans-serif;
    font-weight: 700;
  }

  td {
    padding: 9px 14px;
    border-bottom: 1px solid #e2e8f0;
  }

  tr:nth-child(even) td { background: #f1f5f9; }

  blockquote {
    border-left: 5px solid var(--color-accent);
    background: #eef2ff;
    padding: 16px 24px;
    margin: 16px 0;
    border-radius: 0 8px 8px 0;
    font-style: italic;
    color: #3730a3;
  }

  ul li, ol li { margin-bottom: 8px; line-height: 1.55; }

  section.lead {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  section.lead h1 { font-size: 3em; }

  header, footer {
    font-family: 'DM Sans', sans-serif;
    font-size: 13px;
    color: var(--color-muted);
  }

  /* Two-column layout helper */
  .columns {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 32px;
    align-items: start;
  }

  .columns-3 {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 24px;
  }

  .card {
    background: white;
    border-radius: 12px;
    padding: 20px 24px;
    box-shadow: 0 2px 16px rgba(0,0,0,0.07);
    border-top: 4px solid var(--color-accent);
  }

  .tag {
    display: inline-block;
    background: var(--color-accent);
    color: white;
    border-radius: 99px;
    padding: 2px 12px;
    font-size: 0.7em;
    font-family: 'Syne', sans-serif;
    font-weight: 700;
    letter-spacing: 0.05em;
    text-transform: uppercase;
    vertical-align: middle;
    margin-right: 6px;
  }

  .highlight-box {
    background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);
    color: white;
    border-radius: 12px;
    padding: 20px 28px;
    margin: 12px 0;
  }

  .highlight-box h3 { color: rgba(255,255,255,0.8); }
  .highlight-box p { color: white; margin: 0; }

  section.invert-dark {
    background: #0f172a;
    color: #f1f5f9;
  }
  section.invert-dark h2 { color: #818cf8; border-color: #f59e0b; }
  section.invert-dark blockquote { background: #1e293b; color: #c7d2fe; border-color: #818cf8; }

---

<!--
  ╔════════════════════════════════════════════╗
  ║  SLIDE 1 — TITLE (Lead / Centered layout) ║
  ╚════════════════════════════════════════════╝
-->

<!-- _class: lead -->
<!-- _color: #f1f5f9 -->
<!-- _paginate: false -->
<!-- _header: "" -->
<!-- _footer: "" -->

<span style="font-family:'Syne',sans-serif; font-size:0.75em; color:#6366f1; letter-spacing:0.15em; text-transform:uppercase; font-weight:700;">Academic Research Series · 2026</span>

# Agentic AI for<br>Slide Production

### Automating Presentations with **MCP** & **Claude**

<br>

<span style="font-size:0.75em; color:#94a3b8;">Dr. A. Laurent — AI Systems Lab &nbsp;|&nbsp; Université Paul Sabatier, Toulouse</span>

---

<!--
  ╔══════════════════════════════════════════════════╗
  ║  SLIDE 2 — IMAGE LEFT, TEXT RIGHT (bg left:40%) ║
  ╚══════════════════════════════════════════════════╝
-->

![bg left:42%](https://images.unsplash.com/photo-1677442135703-1787eea5ce01?w=900&q=80)

## What is Agentic AI?

An **agentic system** is an AI that can:

- 🧠 **Reason** over complex, multi-step goals
- 🔧 **Use tools** to interact with the real world
- 🔁 **Iterate** based on feedback and results
- 📋 **Plan** long-horizon workflows autonomously

> "Agentic AI doesn't just answer — it *acts*, *observes*, and *adapts*."

Unlike chatbots, agents **persist** through tasks that span minutes or hours, calling APIs, reading files, and producing structured outputs.

---

<!--
  ╔══════════════════════════════════════════════════╗
  ║  SLIDE 3 — IMAGE RIGHT, TEXT LEFT (bg right:45%)║
  ╚══════════════════════════════════════════════════╝
-->

![bg right:45%](https://images.unsplash.com/photo-1558618666-fcd25c85cd64?w=900&q=80)

## The MCP Protocol

**Model Context Protocol** is an open standard that lets AI models connect to *any* external tool or data source through a uniform interface.

<br>

**Core concepts:**

| Primitive | Role |
|-----------|------|
| `Tools` | Functions the AI can call |
| `Resources` | Data the AI can read |
| `Prompts` | Reusable instruction templates |

<br>

MCP servers expose capabilities; Claude **discovers and orchestrates** them at runtime — no hardcoded integrations.

---

<!--
  ╔═══════════════════════════════════════════╗
  ║  SLIDE 4 — IMAGE TOP (bg top, fit height) ║
  ╚═══════════════════════════════════════════╝
-->

![bg top:50%](https://images.unsplash.com/photo-1639762681485-074b7f938ba0?w=1400&q=80)

<br><br><br><br><br><br>

## Claude as the Orchestrator

Claude acts as the **central brain** of the pipeline — reading intent, calling tools, checking outputs, and iterating until the presentation is complete.

<div class="columns" style="margin-top:12px;">
<div>

**Input:**
- Natural language description
- Topic outline / bullet points
- Brand style guide (optional)

</div>
<div>

**Output:**
- `.md` MARP file (slides)
- Assets folder (images, charts)
- Ready-to-render presentation

</div>
</div>

---

<!--
  ╔═══════════════════════════════════════════════════════╗
  ║  SLIDE 5 — FULL BACKGROUND IMAGE + OVERLAY TEXT      ║
  ╚═══════════════════════════════════════════════════════╝
-->

![bg](https://images.unsplash.com/photo-1451187580459-43490279c0fa?w=1600&q=80)

<!-- _color: #ffffff -->
<!-- _header: "" -->
<!-- _footer: "" -->

<div style="background: rgba(15,23,42,0.72); border-radius:16px; padding: 40px 56px; backdrop-filter:blur(4px);">

# The Big Picture

### From prompt to polished slides — _fully automated_

<br>

**User** → _"Make a 12-slide deck on climate change"_

↓ Claude reasons, plans, calls MCP tools

**Output** → Professional MARP presentation, rendered & ready

</div>

---

<!--
  ╔══════════════════════════════════════════════╗
  ║  SLIDE 6 — TWO-COLUMN TEXT + CODE (HTML div) ║
  ╚══════════════════════════════════════════════╝
-->

## Architecture Overview

<div class="columns">
<div>

**Agent Loop**

1. Receive user prompt
2. Call `plan_slides` tool → outline JSON
3. For each slide, call `generate_content`
4. Call `fetch_image` (Unsplash MCP)
5. Assemble `.md` MARP file
6. Call `render_marp` → PDF / HTML
7. Return download link

<br>

Each step is **observable** and **retryable** — if image search fails, the agent falls back gracefully.

</div>
<div>

```json
// MCP Tool: plan_slides
{
  "name": "plan_slides",
  "description": "Generate slide outline from a topic",
  "inputSchema": {
    "type": "object",
    "properties": {
      "topic": { "type": "string" },
      "slide_count": { "type": "number" },
      "audience": { "type": "string" },
      "style": {
        "enum": ["academic","business",
                 "minimal","creative"]
      }
    },
    "required": ["topic"]
  }
}
```

</div>
</div>

---

<!--
  ╔═══════════════════════════════════════════════════╗
  ║  SLIDE 7 — SPLIT BG (two images side by side)    ║
  ╚═══════════════════════════════════════════════════╝
-->

![bg left:50%](https://images.unsplash.com/photo-1655720828018-edd2daec9349?w=800&q=80)
![bg right:50%](https://images.unsplash.com/photo-1620712943543-bcc4688e7485?w=800&q=80)

<!-- _color: #ffffff -->
<!-- _header: "" -->
<!-- _footer: "" -->

<div style="position:absolute; bottom:60px; left:50%; transform:translateX(-50%); background:rgba(15,23,42,0.85); border-radius:12px; padding:20px 36px; text-align:center; min-width:380px;">

## Without vs With AI

**Manual** — 4–8 hours per deck

**Agentic AI** — _< 3 minutes_

</div>

---

<!--
  ╔═════════════════════════════════════════════════╗
  ║  SLIDE 8 — 3-COLUMN CARD LAYOUT (pure HTML/CSS) ║
  ╚═════════════════════════════════════════════════╝
-->

## Core MCP Tools Used

<div class="columns-3" style="margin-top:24px;">

<div class="card">
<h3>🔍 search_web</h3>

Gathers facts, statistics, and recent citations to enrich slide content automatically.

<br>

**Providers:** Brave, Tavily

</div>

<div class="card">
<h3>🖼️ fetch_image</h3>

Queries Unsplash or Pexels for royalty-free visuals matching each slide's theme.

<br>

**Format:** `?w=1200&q=80`

</div>

<div class="card">
<h3>📊 make_chart</h3>

Generates inline SVG bar, line, and pie charts from structured data — no external tool needed.

<br>

**Output:** Inline `<svg>`

</div>

</div>

<div class="columns-3" style="margin-top:18px;">

<div class="card">
<h3>📁 read_file</h3>
Reads brand guidelines, outlines, or CSV data files from local disk via filesystem MCP.
</div>

<div class="card">
<h3>✍️ write_file</h3>
Writes the final `.md` file to disk. Also saves rendered HTML and PDF exports.
</div>

<div class="card">
<h3>🖨️ render_marp</h3>
Calls `marp-cli` as a subprocess via shell MCP to produce the final slide artifact.
</div>

</div>

---

<!--
  ╔════════════════════════════════════════════════╗
  ║  SLIDE 9 — CODE BLOCK (syntax highlight focus) ║
  ╚════════════════════════════════════════════════╝
-->

## Calling Claude with MCP Tools

```python
import anthropic

client = anthropic.Anthropic()

# 1. Define the MCP-powered tools
tools = [
    {"type": "web_search_20250305", "name": "web_search"},
    # ... custom tools registered via MCP server
]

# 2. Run the agentic loop
messages = [{"role": "user",
             "content": "Create a 10-slide deck on quantum computing for engineers"}]

while True:
    response = client.messages.create(
        model="claude-opus-4-5",
        max_tokens=8192,
        tools=tools,
        messages=messages
    )

    if response.stop_reason == "end_turn":
        break  # ✅ Agent finished — MARP file is ready

    # Process tool calls and append results
    messages = handle_tool_calls(messages, response)

print("Slides generated:", response.content[-1].text)
```

---

<!--
  ╔══════════════════════════════════════════════════════╗
  ║  SLIDE 10 — DARK THEME + QUOTE + TABLE (invert-dark) ║
  ╚══════════════════════════════════════════════════════╝
-->

<!-- _class: invert-dark -->
<!-- _backgroundColor: #0f172a -->

## Benchmark Results

> _"Agentic generation reduced deck production time by **94%** while maintaining professional quality scores above human baseline."_
> — Internal evaluation, AI Systems Lab 2026

<br>

| Method | Time | Quality Score | Cost |
|--------|------|--------------|------|
| Manual (human) | 5.2 h | 8.7 / 10 | €€€€ |
| Template + AI assist | 1.8 h | 8.1 / 10 | €€ |
| **Agentic Claude + MCP** | **4 min** | **8.4 / 10** | **€** |
| Raw LLM (no tools) | 9 min | 6.2 / 10 | € |

<br>

*Quality scored on: coherence, visual balance, content accuracy, citation quality (n=42 decks)*

---

<!--
  ╔════════════════════════════════════════════════════════╗
  ║  SLIDE 11 — IMAGE LEFT + HIGHLIGHT BOXES + TAGS       ║
  ╚════════════════════════════════════════════════════════╝
-->

![bg left:38%](https://images.unsplash.com/photo-1667372393119-3d4c48d07fc9?w=900&q=80)

## Safety & Guardrails

<span class="tag">Critical</span> Agentic systems require layered safety checks at each step.

<div class="highlight-box" style="margin-top:16px;">
<h3>🔒 Prompt Injection Prevention</h3>
<p>All external content (web search, file reads) is sandboxed — Claude never executes raw external instructions as system prompts.</p>
</div>

<div class="highlight-box" style="background: linear-gradient(135deg,#0f766e,#0891b2); margin-top:12px;">
<h3>👁️ Human-in-the-Loop</h3>
<p>Before final render, Claude presents a slide outline for <strong>approval</strong> — ensuring factual accuracy and brand compliance.</p>
</div>

<span class="tag" style="background:#f59e0b;">Tip</span> Always set `max_iterations` on your agent loop to prevent infinite tool calls.

---

<!--
  ╔══════════════════════════════════════════════════════╗
  ║  SLIDE 12 — MULTIPLE INLINE IMAGES IN TEXT GRID      ║
  ╚══════════════════════════════════════════════════════╝
-->

## Visual Layouts MARP Can Produce

<div style="display:grid; grid-template-columns:1fr 1fr 1fr; gap:14px; margin-top:20px; font-size:0.78em; text-align:center;">

<div>
<img src="https://images.unsplash.com/photo-1542744094-3a31f272c490?w=400&q=70" style="width:100%;height:120px;object-fit:cover;border-radius:8px;" />
<strong>Title Slide</strong><br><span style="color:#64748b;">Lead class, centered</span>
</div>

<div>
<img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?w=400&q=70" style="width:100%;height:120px;object-fit:cover;border-radius:8px;" />
<strong>Data Slide</strong><br><span style="color:#64748b;">Tables & code blocks</span>
</div>

<div>
<img src="https://images.unsplash.com/photo-1493612276216-ee3925520721?w=400&q=70" style="width:100%;height:120px;object-fit:cover;border-radius:8px;" />
<strong>Visual Slide</strong><br><span style="color:#64748b;">Full BG image + overlay</span>
</div>

<div>
<img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?w=400&q=70" style="width:100%;height:120px;object-fit:cover;border-radius:8px;" />
<strong>Split Slide</strong><br><span style="color:#64748b;">bg left / bg right</span>
</div>

<div>
<img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?w=400&q=70" style="width:100%;height:120px;object-fit:cover;border-radius:8px;" />
<strong>Card Grid</strong><br><span style="color:#64748b;">3-column HTML layout</span>
</div>

<div>
<img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=400&q=70" style="width:100%;height:120px;object-fit:cover;border-radius:8px;" />
<strong>Quote Slide</strong><br><span style="color:#64748b;">Dark theme + blockquote</span>
</div>

</div>

---

<!--
  ╔══════════════════════════════════════════════════════╗
  ║  SLIDE 13 — IMAGE RIGHT SMALL + STEPPED PROCESS     ║
  ╚══════════════════════════════════════════════════════╝
-->

![bg right:35%](https://images.unsplash.com/photo-1485827404703-89b55fcc595e?w=800&q=80)

## Implementation Roadmap

**Phase 1 — Prototype** <span class="tag" style="background:#22c55e;">Done</span>

Single-agent, MARP output, manual image selection.

**Phase 2 — Tool Integration** <span class="tag" style="background:#f59e0b;">In Progress</span>

MCP servers for web search, image fetch, chart generation, and file I/O.

**Phase 3 — Multi-Agent** <span class="tag" style="background:#6366f1;">Planned</span>

Dedicated sub-agents for: content research · visual design · fact-checking · brand compliance.

**Phase 4 — Platform** <span class="tag" style="background:#64748b;">Future</span>

Web UI, team workspaces, slide version history, one-click render-to-PDF.

---

<!--
  ╔════════════════════════════════════════════════════════╗
  ║  SLIDE 14 — SCOPED STYLE + TIMELINE / VISUAL DIAGRAM  ║
  ╚════════════════════════════════════════════════════════╝
-->

<style scoped>
  section { background: #fafafa; }
  h2 { color: #0f172a; border-color: #6366f1; }
  .step { display:flex; align-items:flex-start; gap:16px; margin:12px 0; }
  .step-num { background:#6366f1; color:white; border-radius:50%; width:36px; height:36px; 
              display:flex;align-items:center;justify-content:center; font-weight:800;
              font-family:'Syne',sans-serif; flex-shrink:0; }
  .step-body { flex:1; }
  .step-body strong { display:block; margin-bottom:2px; }
  .connector { width:2px; height:14px; background:#c7d2fe; margin-left:17px; }
</style>

## Agent Execution Flow

<div class="step">
  <div class="step-num">1</div>
  <div class="step-body"><strong>User Prompt Received</strong>Topic, slide count, audience, style preferences sent to Claude.</div>
</div>
<div class="connector"></div>
<div class="step">
  <div class="step-num">2</div>
  <div class="step-body"><strong>Planning Phase</strong>Claude calls <code>plan_slides</code> → structured JSON outline with titles, bullets, layout types.</div>
</div>
<div class="connector"></div>
<div class="step">
  <div class="step-num">3</div>
  <div class="step-body"><strong>Content Enrichment</strong>Web search + image fetch for each slide — facts, citations, visuals selected.</div>
</div>
<div class="connector"></div>
<div class="step">
  <div class="step-num">4</div>
  <div class="step-body"><strong>MARP Assembly</strong>Slide markdown generated with proper directives, layouts, and embedded images.</div>
</div>
<div class="connector"></div>
<div class="step">
  <div class="step-num">5</div>
  <div class="step-body"><strong>Render & Deliver</strong><code>marp-cli --pdf</code> called via shell MCP. Download link returned to user. ✅</div>
</div>

---

<!--
  ╔══════════════════════════════════════════════════════╗
  ║  SLIDE 15 — CONCLUSION (Lead dark, big text, icon)  ║
  ╚══════════════════════════════════════════════════════╝
-->

<!-- _class: lead -->
<!-- _backgroundColor: #0f172a -->
<!-- _color: #f1f5f9 -->
<!-- _paginate: false -->
<!-- _header: "" -->
<!-- _footer: "" -->

<div style="text-align:center;">

<div style="font-size:3em; margin-bottom:8px;">🚀</div>

# Agentic AI Makes Slide Production *Trivial*

<br>

<div style="max-width:640px; color:#94a3b8; font-size:0.9em; line-height:1.7;">
Claude + MCP turns a natural language description into a complete, rendered, professional presentation in minutes — with web-sourced content, curated visuals, and consistent design.
</div>

<br>

<div style="display:flex; gap:24px; justify-content:center; margin-top:8px;">
  <div style="background:#1e293b;border-radius:10px;padding:12px 24px;font-family:'Syne',sans-serif;font-size:0.75em;color:#818cf8;">📦 MARP + Claude</div>
  <div style="background:#1e293b;border-radius:10px;padding:12px 24px;font-family:'Syne',sans-serif;font-size:0.75em;color:#818cf8;">🔧 MCP Tools</div>
  <div style="background:#1e293b;border-radius:10px;padding:12px 24px;font-family:'Syne',sans-serif;font-size:0.75em;color:#818cf8;">⚡ 4 Minutes</div>
</div>

<br>

<span style="font-size:0.72em; color:#475569;">Questions? · github.com/your-lab/marp-agent · alaurent@ai-lab.fr</span>

</div>