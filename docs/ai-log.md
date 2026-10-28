# AI log

Every time you give an AI tool a significant prompt, add an entry. Three lines each.
"Nothing was wrong" is allowed, but it is rarely true. Your instructor will read this.

## Build 1

### Prompt 1: Build 1 prompt (docs/build-1.md)
- **What I asked:** Implement the terminal-only domain logic from README.md and docs/build-1.md.
- **What came back:** Domain errors, reference IDs, a linked-list queue, inventory rules, and demo/benchmark scripts matching the course requirements.
- **What was wrong (or "nothing"):** The reference generator was named `referenceCode()` instead of the requested `newReference()`, so the implementation and callers were adjusted and a compatibility alias was kept.

## Build 2

### Prompt 1: Build 2 prompt (docs/build-2.md)
- **What I asked:** Add merge sort, event searching/filtering, publish logic, and the first automated tests for S02, S03, S05 and S06.
- **What came back:** A stable merge sort, pure filtering/sorting helpers, publish logic, and `node:test` coverage for the acceptance criteria.
- **What was wrong (or "nothing"):** Nothing major; I checked the behavior against the course rules and confirmed the original list remained unchanged and the sort remained stable.

### Prompt 2:
- **What I asked:** Validate the Build 2 implementation and explain the project test command.
- **What came back:** The suite was reviewed and `npm test` was confirmed as the project’s automated check command.
- **What was wrong (or "nothing"):** Nothing.

## Build 3

### Prompt 1: Build 3 prompt (docs/build-3.md)
- **What I asked:** Add the architecture diagrams, booking state machine, Node HTTP router/server, configuration, startup script, and tests.
- **What came back:** A layered architecture document, explicit booking transitions, static-file HTTP server, `/health` route, startup configuration, and `node:test` coverage.
- **What was wrong (or "nothing"):** The first server draft relied on an implicit response/request property for HEAD handling and had redundant error-status logic; both were simplified. Added a regression test proving static requests cannot escape `public/`.
