# ENVIRA Style Guide

## Writing Conventions

### Voice and Tone
- **Engaged and informed**: Write with authority grounded in evidence, not opinion
- **Urgent but not hyperbolic**: Present the stakes honestly without sensationalism
- **Accessible**: Explain technical concepts for a general educated audience
- **Narrative-driven**: Lead with stories, follow with data, conclude with implications
- **First person sparingly**: Use "we" for shared human stakes; reserve "I" for author's direct experience in foreword/introduction

### Narrative Rules
- **No fictional characters or composite narratives** — every person named must be real and verifiable
- **Real people quoted with attribution** — include context for who they are and why their perspective matters
- **Opening scenes based on documented real events** — cite the source for each opening vignette
- **Speculative statements clearly labeled** — use phrases like "Models project that..." or "Under current trajectories..." rather than presenting projections as fact

### Recurring Characters
The book follows four real people across multiple chapters, giving readers ongoing narratives to track. Each represents a different dimension of the convergence — science, technology, community, and justice. When a recurring character reappears, briefly reintroduce them with a phrase that recalls their earlier appearance (e.g., "Will Marshall, the Planet Labs founder we met in Chapter 3...").

| Character | Role | Chapters |
|---|---|---|
| **Katharine Hayhoe** | Climate scientist and communicator | Ch 1 (profile), Ch 13 (culture shift), Ch 16 (citizen action), Epilogue |
| **Will Marshall** | CEO, Planet Labs | Ch 3 (profile, satellite revolution), Ch 9 (satellite monitoring for restoration), Ch 14 (accountability through data) |
| **Brandon Dennison** | Founder, Coalfield Development | Ch 11 (opening scene + profile), Ch 14 (policy impact on his community), Ch 16 (action, community builder) |
| **Rikki Held** | Lead plaintiff, *Held v. Montana* | Ch 14 (obstacles, legal reckoning), Ch 16 (citizen engagement), Epilogue |

**Guidelines for recurring character appearances:**
- First appearance: full biographical introduction and narrative scene
- Subsequent appearances: brief reintroduction referencing the earlier chapter, then new material — what has changed, what they are doing now, how their story connects to this chapter's theme
- Final appearance (Ch 16 or Epilogue): update on where they stand, closing their narrative arc
- The recurring characters do not replace chapter-specific profiles; they are a narrative thread woven through the book alongside the standalone profiles

### Data Standards
- All quantitative claims must have a cited source
- Prefer peer-reviewed or institutional sources: IPCC, IEA, IRENA, NASA, NOAA, Nature, Science, etc.
- When citing projections, include the source institution and the scenario/assumptions used
- Use conservative estimates; if a range exists, present the range rather than cherry-picking the dramatic end
- **Design capacity vs. operational data:** When citing facility capacities (e.g., DAC plants, renewable installations), always distinguish between *design* capacity (manufacturer/developer claims for fully commissioned operation) and *actual operational* data (verified capture/output). Prefer operational data when available. If only design capacity is available, label it explicitly as such and note that actual performance may differ. Example: Climeworks Mammoth's 36,000 tCO2/year is design capacity; operational capture data (when published) should be cited alongside or instead of the design figure.
- Include date of data publication — climate data changes rapidly
- Round numbers appropriately: "$4.2 trillion" not "$4,200,000,000,000"

### Company-Sourced Data
- Tag all data points originating from the company being profiled with `[COMPANY CLAIM]` in chapter scaffolds
- Do NOT present company-sourced data in the same evidentiary register as peer-reviewed or institutional data
- Use attribution language: "Plenty claims..." or "According to Climeworks..." rather than stating company figures as established facts
- For each `[COMPANY CLAIM]`, assign a verification status: `independently verified`, `partially verified` (press/analyst coverage), or `unverified` (company only)
- Before publication, all `unverified` company claims must either be independently verified or explicitly attributed as company-sourced in the text
- See `research/sources.md` for the full Company-Sourced Data Verification Protocol and tracking table

### Data Freshness Protocol
Climate and energy data changes rapidly. Many figures in this manuscript — solar costs, EV market share, investment totals, installed capacity, battery prices — update annually or more frequently. To prevent staleness at publication:

- **Tag volatile data points** with `[VOLATILE]` in chapter scaffolds. These must be updated during final copy editing to the most recent available figures. Volatile categories include:
  - Energy costs (LCOE for solar, wind, batteries)
  - Investment figures (annual climate tech VC, clean energy investment totals)
  - Market share data (EV adoption rates, renewable energy share of generation)
  - Installed capacity figures (solar GW, battery storage GW, DAC tonnage)
  - Corporate metrics (employee counts, funding raised, facility capacity)
  - Carbon budget remaining (depletes ~40-46 GtCO2/year)
- **Use "as of [date]" qualifiers** for any data point likely to change by more than 10% within a year. Example: "As of 2024, lithium-ion battery pack costs had fallen to approximately $115/kWh (BloombergNEF)."
- **Frame trends over snapshots**: Where possible, emphasize the trajectory rather than a single data point. "Solar costs have fallen by roughly 90% since 2010" is more durable than "$0.044/kWh" alone. Lead with the trend; provide the specific number as supporting evidence.
- **Anchor to structural facts**: Pair volatile numbers with stable underlying facts. "Solar is now the cheapest source of new electricity in most of the world" is more durable than a specific LCOE figure.
- **Distinguish forecasts from targets from projections**: Use precise language:
  - *Projections*: model outputs based on stated assumptions ("IEA projects... under the Stated Policies Scenario")
  - *Targets*: goals set by companies, governments, or organizations ("Climeworks aims to reach megatonne-scale by 2030")
  - *Aspirational targets*: industry-wide cost or performance goals that depend on breakthroughs or favorable conditions — label explicitly as such
  - *Forecasts*: predictions with implied confidence — use sparingly and with attribution
- **Final editing pass**: Before publication, conduct a dedicated data freshness review of all `[VOLATILE]`-tagged figures, updating to the most recent available data from the cited source institutions.

### Chapter Formats

Each chapter specifies one of the following structural formats. Vary formats across consecutive chapters to prevent monotony. See OUTLINE.md for each chapter's assigned format.

1. **Standard narrative**: Opening scene (~500–800 words), context, deep dives (2–4 sections), profiles, challenges, closing bridge. The default.
2. **Data-driven analysis**: No narrative opening. Leads with numbers, uses pullout data boxes, lets the data tell the story. Best for economics, milestones, budgets.
3. **Single extended narrative**: One real event, person, or journey serves as the chapter's spine. All context and data woven around it. Best for human stories.
4. **Profile vignettes**: Shorter sections, each anchored to a specific person or application. Faster pacing, multiple entry points.
5. **Scenario-driven**: Opens with a "what-if" simulation or hypothetical grounded in real data, then unpacks how the technology/system works.
6. **Timeline-driven**: A chronological trajectory (e.g., cost curve, policy evolution) structures the chapter. Past → present → future.
7. **Place-based narrative**: Structured as a journey through 2–3 real locations, each illustrating a different facet of the theme.
8. **Debate format**: Two real perspectives in dialogue. Not a straw man — strongest version of each argument, with synthesis.
9. **Compressed inventory**: No narrative. Direct, dense catalogue organized by type. Short sections, high density. Best for summary chapters.
10. **Audience-segmented guide**: Sections addressed to distinct audiences (entrepreneurs, investors, citizens, policymakers). Each stands alone.

### Interludes

Four interludes appear between parts (~1,500 words each). They break the analytical rhythm with a different register:
- **Dispatch**: First-person field report. Visceral, specific, human-scale.
- **Timeline**: Hour-by-hour or year-by-year. Shows process, not argument.
- **Courtroom narrative**: A real case told as compressed drama. Facts speak.
- **Structured debate**: Two named voices, opposing views, evidence weighed.

### Nervous System Through-Line

The book's central metaphor — Earth gaining a nervous system — must thread from title to epilogue. Every chapter in Parts III–V includes a **"Nervous System Connection"** showing how the planetary sensing/AI/data infrastructure introduced in Part II relates to that chapter's topic. This is not a digression — it's the connective tissue of the book's argument.

### Tensions and Headwinds

Every chapter in Parts III–IV includes a **"Tensions and Headwinds"** section (~500–800 words) that integrates obstacle material directly into the solution context. Present challenges alongside the technologies and initiatives they constrain — not in a separate "obstacles" ghetto.

### AW3 Technology Branding
- AW3 Technology appears **only** in the Author's Note (back matter) and author biography
- The foreword is a personal, intellectually compelling essay — not corporate communication
- The book stands on its own as independent journalism/analysis
- No promotional language for AW3 products or services within chapters or front matter

---

## Citation Format

### In-Text Citations
Use superscript numbers for citations within the text, with full references in the bibliography:

> Global temperatures have risen approximately 1.1°C above pre-industrial levels.¹

### Source Notes
At the bottom of each chapter file, maintain a running list of sources referenced:

```
## Sources
1. IPCC, 2021: Climate Change 2021: The Physical Science Basis. AR6 Working Group I.
2. NASA GISS, 2024: Global Temperature Record. https://data.giss.nasa.gov/gistemp/
```

### Bibliography Entry Format
Follow Chicago Manual of Style (17th edition) for the full bibliography:

- **Journal article**: Author(s). "Title." *Journal Name* Volume, no. Issue (Year): Pages. DOI.
- **Report**: Organization. *Title*. Place: Publisher, Year. URL.
- **Book**: Author(s). *Title*. Place: Publisher, Year.
- **Web source**: Author/Organization. "Title." Website Name. Date. URL.

---

## Formatting Conventions

### Headings
- Chapter title: `# Chapter N: Title`
- Major sections: `## Section Title`
- Subsections: `### Subsection Title`

### Numbers
- Spell out one through nine; use numerals for 10 and above
- Always use numerals with units: 2°C, 415 ppm, $3.4 trillion
- Use commas in numbers over 999: 1,000 not 1000
- Use "billion" and "trillion" rather than scientific notation for general audience

### Units
- Temperature: Celsius (with Fahrenheit in parentheses on first use per chapter)
- Currency: USD unless otherwise specified; note conversion date for other currencies
- Energy: Use the unit most common in the source (GW, TWh, etc.) and define on first use
- Emissions: metric tons CO2 equivalent (tCO2e); gigatons for global figures (GtCO2e)

### Names and Terms
- On first use: full name with brief identifier — "Christiana Figueres, the former UNFCCC Executive Secretary"
- Subsequent uses: last name only
- Acronyms: spell out on first use per chapter with abbreviation in parentheses
- Technical terms: define on first use; include in glossary

### Emphasis
- *Italics* for book titles, ship names, species names, and introducing key terms
- **Bold** sparingly, for critical emphasis only
- Avoid ALL CAPS for emphasis

---

## Chapter File Template

```markdown
# Chapter N: [Title]
## [Subtitle]

**Part**: [Part name]
**Target word count**: X,000 words
**Format**: [Format name from Chapter Formats list]

---

## [Opening — varies by format]
[Standard narrative: real event/person/place. Data-driven: lead numbers.
 Single narrative: introduce the protagonist. Etc.]

---

## [Section 1 Title]
[Content notes, key points to cover]

### Key Data Points
- [Data point with source]

### Profiles
- [Real person/company/organization to feature]

---

## [Section 2 Title]
...

---

## Nervous System Connection
[How sensing/AI/data infrastructure relates to this chapter's topic.
 Required for all chapters in Parts III–V.]

---

## Tensions and Headwinds
[Obstacles and challenges integrated into solution context.
 Required for all chapters in Parts III–IV. ~500–800 words.]

---

## Sources
1. [Source citation]
2. [Source citation]
```

## Interlude File Template

```markdown
# Interlude: [Title]

**Format**: [Dispatch / Timeline / Courtroom narrative / Structured debate]
**Target word count**: ~1,500 words
**Placement**: After Part [N]

---

[Content — no sections, no data boxes. A single sustained piece
 in a different register from the analytical chapters.]

---

## Sources
1. [Source citation]
```
