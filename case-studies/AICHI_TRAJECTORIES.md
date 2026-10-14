# Aichi: bounded conversational trajectories

**Status:** Early-system project account and architectural interpretation, clarified by Troy Vance Williams on October 14, 2026. Public implementation excerpts are not included in this edition.

## The engineering idea

Aichi explored a practical observation: many business-reception calls follow a limited set of recurring trajectories. The words can vary while the underlying task remains recognizable—answer a question, arrange a booking, collect a missing detail, handle a detour, or finish the call.

The architectural response was a stateful kernel that selects the relevant behavior and carries the interaction forward. The useful object is the conversation's trajectory: where the caller is trying to go, what has already happened, and what should happen next.

This is Vance's account of the design insight. It is not a measured claim that every business conversation fits a fixed menu, or that identifying a trajectory eliminates the need to handle ambiguity.

## What Vance reports from operation

Vance describes the early Aichi system as a realistic, fast receptionist that worked on consumer-grade hardware. That is an operational account from the person directing and using the project. It should be preserved as such, alongside the architecture that made the experience possible.

The portfolio audit found source code consistent with a context-driven kernel selecting skills and advancing the call lifecycle, and later specifications organizing conversation families and detours. Those implementation sources remain private.

No numerical latency or concurrency claim is made here. “Consumer-grade hardware” identifies the reported host environment; it does not establish that every speech, language, or telephony component ran locally.

## Development lineage

| Stage | Contribution | Evidence status |
| --- | --- | --- |
| Early Aichi receptionist | Apply kernel-directed conversation flow to a practical business task | Vance's operational account; relevant private implementation inspected |
| Explicit trajectory modeling | Describe recurring flows, detours and returns so behavior can be inspected | Private specifications and code located; public extract pending |
| Hardware follow-on | Explore carrying this approach into a specialized chip | Vance reports later design work; design artifacts and maturity not yet verified in this audit |

The hardware follow-on is a separate design artifact to recover and examine. This account does not imply fabrication, a working chip, or measured hardware performance.

## Why it belongs in the portfolio

Aichi contributes an engineering example of choosing a representation that fits a bounded task. It suggests a research question: how much useful interaction can be carried by explicit state and trajectories, and when does the system need a different path or more general reasoning?

A demonstration of usefulness can precede a formal benchmark. The public case should recover that operational history and the design decisions, then attach the strongest available artifacts. Current CI status is a different question from whether an earlier version worked in practice.

## Next evidence to recover

Locate existing hardware/setup records, non-sensitive demonstrations, and the later chip design before deciding what new demonstration is necessary. A release should distinguish the early software, later trajectory instrumentation, operational observations, and hardware design maturity.

**Source for the project account:** Vance's October 14, 2026 clarification during the portfolio review. The private audit retains exact implementation pointers. This page is a transparent project account, not a publicly reproducible implementation package.
