# Brandon Baker

**Software engineering · Deterministic systems · Developer infrastructure**

I build software that can explain where its answers came from.

My current focus is a reusable foundation for turning complex written rules - regulations, rule-books, and other authoritative material - into deterministic, testable software. The goal is not just to produce an answer, but to preserve the chain from the source, through interpretation and implementation, to the behavior a user can verify.

My background spans enterprise IT, systems administration, application development, and automation. That experience shapes how I approach software: clear boundaries, reproducible builds, useful tests, and systems designed to be operated and maintained.

## What I'm building

The central project is a **source-backed rules-engine ecosystem**. Its components separate work that is often conflated:

```text
Authoritative source material
            |
            v
Reproducible, verifiable corpus
            |
            v
Evidence-backed rule map <--- independent validation
            |
            v
Generated contracts + domain-specific implementation
            |
            v
Deterministic rules engine
            |
            +--> APIs and business applications
            +--> Interactive games and simulations
            +--> AI opponents and evaluation tools
```

A source document is not executable code, and a generated contract is not proof that the underlying rule has been implemented correctly. The architecture is designed around that distinction: source provenance, explicit interpretation, independent checks, reproducible execution, and honest handling of unresolved cases.

### Public projects

| Repository | What it does |
| --- | --- |
| [**rules-factory**](https://github.com/brandonifco/rules-factory) | Maps and validates documented rules, then produces the generated contracts, provenance, and verification infrastructure for domain-specific .NET engines. |
| [**rules-corpus**](https://github.com/brandonifco/rules-corpus) | Builds reproducible, verifiable, content-addressed corpora from authoritative source material without interpreting the rules themselves. |
| [**rules-kernel**](https://github.com/brandonifco/rules-kernel) | Supplies ruleset-agnostic identity, provenance, deterministic randomness, replay support, and explicit resolution contracts. |
| [**FAA Part 107**](https://github.com/brandonifco/faa-part-107) | Applies the architecture to a defined scope of U.S. small-drone regulations, with traceable regulatory citations. |
| [**Hoyle Backgammon**](https://github.com/brandonifco/hoyle-backgammon) | Implements a deterministic game engine grounded in a public-domain 1909 rulebook. |
| [**SRD 5.2.1 Combat**](https://github.com/brandonifco/srd-52-combat) | Implements mapped portions of tabletop combat rules, with explicit source references and reproducible random outcomes. |
| [**The Hollow Crown**](https://github.com/brandonifco/hollow-crown) | An independent, browser-based action-adventure project combining gameplay systems, procedural generation, art, and audio. |

These repositories show the same engineering approach across different domains—not a claim that all rules, edge cases, or possible applications have been completed.

## Current areas of development

Alongside the public infrastructure, I'm developing and evaluating:

- **Applications built on authoritative engines:** API and browser experiences that present decisions without reimplementing the rules in the user interface.
- **Game-independent AI:** opponent policies, search, conformance checks, and strength/latency calibration, with legality determined by the underlying engine.
- **Measured, agent-assisted engineering:** repeatable development workflows, independent review, validation gates, and experimental measurement of both output quality and computational cost.
- **Domain-specific software:** ways to apply the same architecture to regulatory questions, operational workflows, tabletop systems, and other rules-intensive products.

Some of this work is in private repositories or remains experimental. I prefer to distinguish demonstrated capabilities from development goals.

## Engineering principles

- **Evidence before assertions.** Preserve sources, versions, citations, and the boundary between written authority and an implementer's decision.
- **Determinism where it matters.** Given the same inputs and decisions, a rules engine should support reproducible outcomes and replay.
- **Verification beyond a green build.** Use independent checks, regression tests, mutation testing, and explicit acceptance criteria appropriate to the claim being made.
- **Clear responsibility between layers.** An engine decides what is legal or applicable; a UI presents it; an AI policy chooses among permitted actions.
- **Explicit limits.** When source material is ambiguous, incomplete, or outside scope, the software should say so rather than invent certainty.
- **Automation with accountability.** AI can accelerate engineering, but generated work still needs bounded processes, traceable evidence, and review.

## Where I'm headed

My long-term aim, through **Man-Made Brains Studios, LLC**, is to turn this engineering foundation into practical, maintainable products—not a collection of one-off prototypes.

I want to make complex systems easier to build, integrate, test, and trust. That means reusable infrastructure beneath applications that solve real problems, with the source of a decision and the limits of the software visible to the people relying on it.

## Background and tools

**Primary development:** C# / .NET, Python, JavaScript, PHP, SQL, Bash, REST APIs, and web technologies.

**Engineering environment:** Linux, Git and GitHub, CI/CD, automated testing, systems integration, infrastructure, and operational troubleshooting.

My work combines hands-on software development with experience running and supporting real-world IT systems.

## Connect

I'm interested in conversations about rules engines, developer tooling, evidence-driven applications, and practical software products.

**Email:** [brandonifco@gmail.com](mailto:brandonifco@gmail.com)
