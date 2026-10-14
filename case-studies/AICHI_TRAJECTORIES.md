# Aichi: bounded conversational trajectories

**Status:** Early-system project account, with an illustrative hardware extension. Operational experience and the product decision are attributed to Troy Vance Williams's October 14, 2026 account.

## The engineering idea

Aichi explored a practical observation: many business-reception calls follow a limited set of recurring trajectories. The words can vary while the underlying task remains recognizable—answer a question, arrange a booking, collect a missing detail, handle a detour, or finish the call.

The architectural response was a stateful kernel that selects the relevant behavior and carries the interaction forward. The useful object is the conversation's trajectory: where the caller is trying to go, what has already happened, and what should happen next.

## What the work accomplished

Vance describes the early Aichi system as a realistic, fast receptionist that worked on consumer-grade hardware. Its central engineering takeaway was the use of a kernel to choose among recurring conversational paths.

The portfolio audit inspected private source code implementing context-driven skill selection and call-lifecycle updates, together with specifications describing conversation families, detours, and returns. This supports the architectural account. Responsiveness and the consumer-hardware experience remain qualitative operational observations from Vance.

## Why work stopped

Work on the receptionist product stopped because Vance judged that it no longer appeared to be a product the future needed.

The lasting contribution was the trajectory-based way of thinking: represent the task's recurring paths, preserve the context needed to choose among them, and carry the interaction toward a useful outcome.

## A possible hardware extension

At the architectural level, a chip carrying the trajectory-selection mechanism is straightforward to envision. A small controller could store the current interaction state, apply transition or selection rules to incoming signals, and dispatch the next action. Speech interpretation could supply those signals, while the controller carries the bounded interaction structure.

This is an illustrative hardware concept, scoped to trajectory selection. It expresses a possible extension of the software idea.

## Why it belongs in the portfolio

Aichi contributes an engineering example of choosing a representation that fits a bounded task. It suggests a research question: how much useful interaction can be carried by explicit state and trajectories, and when does the system need a different path or more general reasoning?

It also records a product judgment: deciding where to stop investing while retaining what the work taught.

**Sources and attribution:** Vance's October 14, 2026 clarifications supply the operational account, design insight, and reason for stopping. The private audit retains exact implementation pointers. The hardware paragraph is an AI-assisted architectural illustration prepared for this portfolio at Vance's direction.
