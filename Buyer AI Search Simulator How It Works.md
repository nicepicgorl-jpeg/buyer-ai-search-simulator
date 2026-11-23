# Buyer AI Search Simulator: How It Works

Nov 23, 2026 · @Bishal Mukherjee

This is the reference behind the sales page: how evidence is labelled, how tools are discovered and what each report contains.

## Evidence labels

Every meaningful finding carries one of seven labels, so a reader can tell what was measured from what was generated.

| Label | Meaning |
| --- | --- |
| SUPPLIED | Information provided by the user, the brand or an uploaded dataset |
| OBSERVED | Information found directly in an external source reviewed during the task |
| VALIDATED | A finding supported by relevant research or quantitative evidence |
| INFERRED | A reasonable interpretation of available information |
| SIMULATED | Generated personas, queries and hypothetical conversations |
| UNKNOWN | Information that cannot currently be established |
| NOT TESTED | Research or visibility tests that were planned but not performed |

A simulated or inferred finding is never promoted to VALIDATED without new evidence.

## Evidence ledger

Research and Full Intelligence reports keep a ledger so important findings can be traced to their support. Each entry records:

- Evidence ID and the finding
- Evidence label
- Source or provider, and the source URL where available
- Collection date and geography
- Metric and exact value
- Confidence level and research limitations
- Related query, prompt and recommendation IDs

IDs match between the written report and any spreadsheet export.

## Capability discovery and confidence

In Research and Full Intelligence modes, the skill checks what your environment can do before it starts. It maps the tools it finds to eight capabilities, tests them with real calls, and tells you what it will use and skip.

| Capability | Needed for | If unavailable |
| --- | --- | --- |
| Web search | Market, brand and competitor research | External claims stay UNKNOWN |
| Page extraction | Inspecting actual page content | No claims about page content |
| Keyword metrics | Quantitative demand validation | Demand stays unvalidated |
| SERP data | Search-result and competitor analysis | SERP analysis is skipped |
| Trend data | Seasonality and interest patterns | Seasonality claims are omitted |
| Review and community access | Buyer language and objections | Buyer language stays SIMULATED |
| AI platform access | Live visibility testing | Tests stay NOT TESTED |
| First-party analytics | Actual brand search performance | No performance claims |

Each capability used is then labelled:

- **Live:** a real call succeeded during this task.
- **Supplied historical:** the data came from a user-provided export and reflects its collection date.
- **Partial:** the capability worked only in part, for example volume without difficulty, one country, or truncated results.

These labels appear in the disclosure before research and in the methodology section, and a conclusion is never stated more firmly than its weakest input.

## Data freshness and provider conflicts

**Freshness.** The report records two dates separately: when the data was collected and when the report was generated. For uploaded files, the collection date is kept apart from the save date, and it is marked UNKNOWN if it cannot be established. By default, keyword and SERP data older than about 90 days and AI-assistant outputs older than about 30 days are flagged for review. Older data can still be used, but it is labelled historical. These are adjustable defaults.

**Conflicts.** When two providers disagree on a metric, both values are shown with provider, date and settings. They are never averaged. The report lists plausible causes: different keyword databases, geography or language settings, volume definitions, collection dates, or device and SERP settings. If the cause cannot be established, the disagreement stays unresolved. Where a recommendation depends on the disputed figure, the report shows how it changes under each value.

## Deliverables and research depth

What you get depends on the mode and the tools available.

| Deliverable | What it contains |
| --- | --- |
| Brand fact sheet | Brand details, products, differentiators and unknowns |
| Buyer personas | Audience segments, needs, motivations and objections |
| Buyer journey map | Discovery, evaluation, comparison and purchase stages |
| Search query library | Categorized Google-style queries with intent, stage and evidence label |
| AI prompt library | Context-rich prompts with follow-ups |
| Simulated conversations | Multi-turn buyer research scenarios |
| Competitor intelligence | Positioning, products, pricing and content comparisons, where researched |
| Keyword research | Demand metrics, where a provider or export supplies them |
| Priority test set | High-value queries and prompts to validate |
| Visibility test log | Brand mentions, competitors, citations and accuracy, where tested |
| Content opportunities | Recommendations linked to buyer needs and evidence IDs |
| Evidence ledger | Sources, dates, geography, metrics and confidence |

Three depths are available. The counts are targets, not guaranteed output.

| Depth | Google-style queries | AI prompts | Simulated conversations | Priority tests |
| --- | --- | --- | --- | --- |
| Quick | about 40 | about 30 | 3 | 10 |
| Standard | about 100 | about 80 | 5 | 20 |
| Comprehensive | about 200 | about 150 | 8 | 30 |

## Worked example: a premium dog food brand in India

A conventional keyword exercise gives you phrases like "best dog food in India", "premium dog food" and "dog food for sensitive stomachs". The skill looks at the buyer behind them:

- What does a first-time owner need to know before choosing a premium food?
- What makes an experienced owner distrust a dog food label?
- How do buyers compare ingredient transparency?
- Which product claims need stronger evidence?
- Which questions would someone ask an AI assistant instead of Google?

A multi-turn AI test then follows a buyer as they narrow down:

1. What are the best premium dog food brands in India?
2. Which brands provide transparent ingredient information?
3. What should I look for when choosing food for a dog with a sensitive stomach?
4. Which products would you compare?
5. What evidence should I look for before buying?

Simulation Mode produces the questions as labelled hypotheses. Research Mode checks them against search data, competitor content and public discussions. Full Intelligence Mode tests whether the brand appears in AI recommendations, where the platforms can be reached.

*This example is illustrative and is not a real client run.*
