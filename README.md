
# Westlee Latta

Technical program manager working on developer platforms and AI tooling. AI as a force multiplier, not a replacement for people, process or meaningful artifacts.

## Projects

### [program-risk-backtest](https://github.com/wblatta/program-risk-backtest)
Can you tell which planned work is going to slip, early enough to do something about it, using only the artifacts teams already produce?

This answers that with a measurement rather than an opinion. It reconstructs what the Kubernetes roadmap said on every date across nineteen release cycles, asks four candidate risk signals what they thought on each of those dates, and scores them against what actually happened. The fourth signal is the release team's own scope label, included as a control, on the principle that a signal which cannot beat the judgment an organisation already writes down is not worth building.

On 1,255 committed deliverables across six years: silence predicts slippage about as well as the release team's own label does, the two find different failures, and together they flag 7% of committed work at 92% precision eight weeks before the deadline. Then the project stopped applying that label. The conjunction disappeared with it. The activity signal kept working unchanged.

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
