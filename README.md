# ASEAN Cybersecurity Market Outlook 2026-2028

A 16-slide market outlook for **six ASEAN countries** (Singapore, Malaysia, Indonesia, the Philippines, Vietnam and
Thailand): market size and growth, the industries that spend most, the main threats and the new laws driving
budgets. The deck is **generated from data by a Python script**, and every figure traces to a named source and
edition in a source ledger.

![Cover](images/slide-01.png)

## What's inside
- **Slides 1-7:** how to read the deck, the regional market at a glance, market size by country, threat and
  technology trends, regulation.
- **Slides 8-13:** one profile per country: size and growth, top industries, biggest threat, rules to know.
- **Slides 14-16:** all six countries side by side, takeaways (labelled as opinion), sources.
- **Headline:** the ASEAN market grows from US$5.51B (2025) to US$14.10B (2031 forecast), a CAGR of ~17%
  (Mordor Intelligence).
- Every slide has a source line and speaker notes.

![The ASEAN market at a glance](images/slide-03.png)

## How it's built
- [`build_deck.py`](build_deck.py) holds the figures as Python data and draws every slide with python-pptx. The six
  country profiles are one template looped over six records, so a figure is edited in one place.
- Charts are native PowerPoint charts, so their data stays inside the `.pptx` and anyone can check it.
- [`sources.md`](sources.md) records every figure with its value, source and edition, plus a change log from the
  monthly re-checks. One market-size source covers all countries so they can be compared; Malaysia's wider
  definition is flagged wherever it appears.
- Order of work: ledger first, then the script, then rebuild. The figures are the baseline as of 1 October 2026.

## Open it
- Read the [PDF](ASEAN_Cybersecurity_Outlook_2026-2028.pdf) or open the
  [PowerPoint deck](ASEAN_Cybersecurity_Outlook_2026-2028.pptx).
- Rebuild it: `pip install python-pptx`, then `python build_deck.py`.

**Tools:** Python (python-pptx), Markdown source ledger, PowerPoint · built with Claude Code as a coding assistant
