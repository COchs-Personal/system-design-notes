# Source reference

This handbook describes committed source in COchs-Personal/system-design-notes at `d3f6b41b2507f8ec835a070ce53743651ecaab95`. Paths below are relative to this repository. Source-defined behavior is distinguished from a fresh runtime verification; no application or game was launched to author these chapters. The existing quick operating guide remains available separately.

## Reading the evidence

A source file explains what the program is designed to do. A test states an expectation and may exercise only one layer. A README describes an intended workflow and can lag implementation. When these disagree, inspect the exact revision and the executable code, reproduce the disagreement in a safe local test, and correct the relevant documentation with the change. Do not treat a passing unit test as proof of rendering, sound, external connectivity, deployment, or save recovery.

## File and symbol index

| File | Responsibility | Entry points and locations |
|---|---|---|
| [Readme.md](https://github.com/COchs-Personal/system-design-notes/blob/d3f6b41b2507f8ec835a070ce53743651ecaab95/Readme.md) | Root topic index, attribution and further reading | L1 to L101 |
| [04. Rate Limiter/Readme.md](https://github.com/COchs-Personal/system-design-notes/blob/d3f6b41b2507f8ec835a070ce53743651ecaab95/04.%20Rate%20Limiter/Readme.md) | Algorithm comparisons and distributed considerations | L1 to L132 |
| [07. Unique-Id Generator/Readme.md](https://github.com/COchs-Personal/system-design-notes/blob/d3f6b41b2507f8ec835a070ce53743651ecaab95/07.%20Unique-Id%20Generator/Readme.md) | Requirements, alternatives and Snowflake-style example | L1 to L100 |
| [12. Chat System/Readme.md](https://github.com/COchs-Personal/system-design-notes/blob/d3f6b41b2507f8ec835a070ce53743651ecaab95/12.%20Chat%20System/Readme.md) | Hypothetical chat requirements, flows, storage and presence | L1 to L204 |
| [21. Ad Click Event Aggregation/README.md](https://github.com/COchs-Personal/system-design-notes/blob/d3f6b41b2507f8ec835a070ce53743651ecaab95/21.%20Ad%20Click%20Event%20Aggregation/README.md) | Aggregation study chapter and design discussion | L1 to L549 |

## Keeping the handbook useful

When code changes, update the chapter that explains its contract, the relevant diagram, the change recipe, and this pinned source register. Keep the Word and PDF editions synchronized with the Markdown chapters. Record what was actually tested, what remained unverified, and which saved data must survive an upgrade. A future maintainer should be able to trace an instruction to a file or a test without relying on a previous conversation.
