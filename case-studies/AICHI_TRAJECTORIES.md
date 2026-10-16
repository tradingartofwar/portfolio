# Aichi: bounded conversational trajectories

**Status:** Early-system project account, with an illustrative hardware extension. Operational experience and the product decision are attributed to Troy Vance Williams's October 14 and October 16, 2026 accounts. Claim IDs: P-007–P-009.

## The engineering idea

Aichi explored a practical observation: many business-reception calls follow a limited set of recurring trajectories. The words can vary while the underlying task remains recognizable—answer a question, arrange a booking, collect a missing detail, handle a detour, or finish the call.

The architectural response was a stateful kernel that selects the relevant behavior and carries the interaction forward. The useful object is the conversation's trajectory: where the caller is trying to go, what has already happened, and what should happen next.

In his October 16 telling, Vance names this **trajectory intelligence** and emphasizes bounded options, detours, and returns to the original path. The architectural description concerns interaction state and selection; modification of the host operating system's kernel has not been established.

## What the work accomplished

Vance describes the early Aichi system as a realistic, fast receptionist that worked on consumer-grade hardware. Its central engineering takeaway was the use of a kernel to choose among recurring conversational paths.

His October 16 account supplies the practical use: an office assistant responding to a workplace need could answer calls, check schedules, make appointments, and send relevant information to a therapist in another language. He recalls using Whisper and ElevenLabs, with natural-sounding voice and real-time interaction hosted on his usual laptop. These are reported functions and qualitative impressions, without fresh runtime checks or measured latency. The laptop is the reported host; the complete local/cloud processing split has not been verified. His explanation credits the bounded trajectory design, but no comparative performance test is supplied.

The portfolio audit inspected private source code implementing context-driven skill selection and call-lifecycle updates, together with specifications describing conversation families, detours, and returns. This supports the architectural account. Responsiveness and the consumer-hardware experience remain qualitative operational observations from Vance.

## Why work stopped

Work on the receptionist product stopped because Vance judged that it no longer appeared to be a product the future needed. He clarified on October 16 that he expected GPT or similar general assistance to provide this functionality for free in the near future. This records his judgment at the time, not an established product forecast.

The lasting contribution was the trajectory-based way of thinking: represent the task's recurring paths, preserve the context needed to choose among them, and carry the interaction toward a useful outcome.

## A possible hardware extension

At the architectural level, a chip carrying the trajectory-selection mechanism is straightforward to envision. A small controller could store the current interaction state, apply transition or selection rules to incoming signals, and dispatch the next action. Speech interpretation could supply those signals, while the controller carries the bounded interaction structure.

This is an illustrative hardware concept, scoped to trajectory selection. It expresses a possible extension of the software idea.

## Why it belongs in the portfolio

Aichi contributes an engineering example of choosing a representation that fits a bounded task. It suggests a research question: how much useful interaction can be carried by explicit state and trajectories, and when does the system need a different path or more general reasoning?

It also records a product judgment: deciding where to stop investing while retaining what the work taught.

**Sources and attribution:** Vance's October 14 and October 16, 2026 clarifications supply the operational account, design insight, and reason for stopping. The earlier private audit retains its implementation pointers; the October 16 additions are retrospective testimony, not a repeat of that audit. The hardware paragraph is an AI-assisted architectural illustration prepared for this portfolio at Vance's direction. [The broader development account](FROM_CAPABILITY_TO_PARTICIPATION.md) connects this work to later collaboration and networking questions.
