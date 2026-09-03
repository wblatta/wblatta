
# Westlee Latta

Technical program manager working on developer platforms and AI tooling. AI as a force multiplier, not a replacement for people, process or meaningful artifacts.

## Projects

### [program-risk-backtest](https://github.com/wblatta/program-risk-backtest)
Can you tell which planned work is going to slip, early enough to do something about it, using only the artifacts teams already produce?

What it is. An event-sourced backtest of delivery risk. It replays what the Kubernetes roadmap said on every date across 19 release cycles, asks ten candidate signals what they thought at each date, and scores them against outcomes they could not have seen. 1,255 committed deliverables, 2020–2026.

The result. Two independent checks - nobody has touched the work in eight weeks and the required approval gate has no holder - agree on 12% of committed work and are right about 94% of it, eight weeks before the deadline. That significantly beats either alone and beats the release team's own scope label.

The catch. It misses three quarters of all slips. Precision is high, recall is low. A triage tool, not a safety net.

The uncomfortable finding. For three consecutive cycles the release team stopped applying its own scope label entirely, and did not appear to notice. Signals reading what people did got stronger through that period; the one reading what people recorded got weaker.

Reported failures. Of ten signals, four carry real information, four are indistinguishable from noise, one is significantly negative (work committed late slipped less), and one pair could not be tested at all. All three pre-registered hypotheses got a verdict, including the one that failed.

No model, by design. LLMs were scoped for extraction, not prediction - and the extraction path was built and measured. Its ceiling is the corpus, not the technique.

Why one corpus. 41 candidate projects were measured before declining to build a second. Only three non-Kubernetes projects clear the bar, and all three copied the Kubernetes process.

Six errors, published. Including one that meant an early draft drew conclusions from 6% of the available data. The corrections are in docs/findings.md, and they are more instructive than the result.

Python.

### [tpm-hub](https://github.com/wblatta/tpm-hub)
A mission control surface for technical program managers.

This is a presentation scaffold: a portfolio demo of Cerebro, a local-first tool I built and used daily as a TPM at Netflix. The UI is real and fully interactive. The data is mocked, with no live integrations, no database, and no model calls.

It demonstrates one workflow. Sync, generate insights, review them in an inbox that acts as a human-in-the-loop gate, then publish. Nothing a model produces reaches another system without a person approving it. Every generated artifact carries its provenance, meaning the specific threads, issues, pages, calendar events, and pull requests it was synthesized from.

TypeScript. Live at [wblatta-tpm-hub.dreamhosters.com](http://wblatta-tpm-hub.dreamhosters.com)

### [lakecitycommons](https://github.com/wblatta/lakecitycommons)
Neighborhood news and community site for Lake City, Seattle, running in production at [lakecitycommons.com](http://www.lakecitycommons.com). Grew out of OlyHillsHub, a referral-only time-banking and item-sharing platform that is still in the codebase behind a feature flag.

Laravel 12, MySQL, Blade, Tailwind, Alpine.

### [retroEd](https://github.com/wblatta/retroEd)
A small Markdown word processor for macOS with CRT phosphor and Classic Mac themes. Plain `.md` files in a folder you choose, so there is no lock-in and syncing is whatever you already use.

TypeScript.
