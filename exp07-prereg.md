COMMON GROUND EXPERIMENT 07 — EVIDENCE CONFLICT GATE
PREREGISTERED DESIGN • SYNTHETIC • NOT RESEARCH EVIDENCE


PURPOSE
Experiment 06 established that Controller v2 validates arithmetic against trusted configuration but cannot independently establish source truth. Experiment 07 tests a SEPARATE, deterministic evidence gate against real Drive-hosted synthetic fixture documents. It is not a Controller v2 upgrade, not autonomous semantic reasoning, and not independent agent cooperation.


EXPERIMENTAL SUBJECT
Topic: household_discretionary_budget. Source A asserts 120000 cents; source B asserts 200000 cents. Source C repeats 120000 cents with the same declared lineage as A. Source D independently declares 120000 cents under a different fictional lineage. All numbers and metadata are invented; timestamps, status labels and lineage claims in the documents are untrusted until authenticated externally.


FROZEN PREDICTIONS (before any execution)
01. A+B disagree in budget amount -> HOLD:CONFLICTING_VALUES.
02. A+C agree but share declared lineage -> HOLD:CORRELATED_SOURCES.
03. A+D agree with distinct declared lineage -> REVIEW_ONLY:CONSISTENT_UNVERIFIED (not verified).
04. A alone -> HOLD:SINGLE_SOURCE.
05. A listed twice -> HOLD:DUPLICATE_SOURCE_ID.
06. Tampered expected source hash (simulated only; documents unchanged) -> HOLD:HASH_MISMATCH.
07. Embedded instruction in B demanding that the controller override rules is ignored by a whitelist parser; A+B remain held.
08. Even though A declares CURRENT and B declares ARCHIVED, their self-described timestamps/statuses never automatically override the conflict -> HOLD.
09. Existing Controller v2 accepts a structurally valid $1,600 spend with the WRONG $2,000 configured pool; the separate evidence gate still holds A+B as conflicting. THIS IS A COMPARISON, NOT INTEGRATION.
10. Real execution remains disabled -> HOLD:REAL_EXECUTION_DISABLED.


METHOD
Create synthetic Docs in the pre-existing CommonGround folder. Use cgrRead_ from installed Controller v2 to read and hash; parse only explicitly prefixed CG07_ fields with a deterministic regex. Never interpret ordinary prose as code, authority, or instructions. Run testCGExp07EvidenceConflict manually as a separate Apps Script file. Save full JSON result to CommonGround folder and write one TEST ONLY row in Revision Log. Compare trusted Nodes, Edges, Claims, Audit Queue before and after. No deployment, triggers, new permissions, CGR_TASKS_V2 updates, real actions, or edits to controller code.


PASS CRITERION
Ten predictions match, all four source texts remain stable during the test, trusted graph data is unchanged, no fatal error. A pass supports the implemented deterministic test harness only; it does not establish that Controller v2 already has semantic conflict detection or independently authenticated provenance.


LIMITATIONS / NEXT RESEARCH
Self-declared lineages can be falsified. Matching values are not proof of truth. Parsing a structured claim key is not general natural-language contradiction detection. The test assumes a human defined common claim type and wrote expected outputs; no blind gold set, randomized unseen claims, independent adjudication, authenticated multi-agent transport, or measurable end-to-end decision improvement. The controller remains separate from this experimental gate.


STATUS
FIXTURES CREATED; EXECUTION NOT YET RUN. This document freezes expected results prior to human-run Apps Script execution. Results must be checked against actual JSON and Revision Log and recorded as OBSERVED, INFERRED or PROPOSED.
