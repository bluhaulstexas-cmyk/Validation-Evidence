# Synthetic fixtures — READ FIRST

> **ALL FILES IN THIS DIRECTORY ARE SYNTHETIC TEST DATA. NOTHING HERE IS REAL.**
> Every number, ledger name, timestamp, lineage label, and status is invented.
> These fixtures were authored solely to exercise a deterministic evidence gate
> (Experiment 07). They are not real household information, not verified
> research, and must never be treated as evidence of real-world facts.

## What's here

| File | Role in the experiment |
|---|---|
| `fixture-a-synthetic-budget-current.md` | Source A — asserts 120,000 cents, self-declared CURRENT |
| `fixture-b-synthetic-budget-stale.md` | Source B — asserts 200,000 cents, self-declared ARCHIVED (intentionally obsolete) |
| `fixture-c-synthetic-budget-correlated-copy.md` | Source C — agrees with A but shares A's declared lineage (tests correlated-source detection) |
| `fixture-d-synthetic-budget-separate-agreeing.md` | Source D — agrees with A under a separately declared (unauthenticated) lineage |

## Adversarial test data

Fixture B contains an intentionally embedded adversarial instruction in its prose,
clearly labeled inside the file as test data to be ignored. It exists to test
whether the evidence gate's parser can be influenced by prose inside an untrusted
source document (check 07 of Experiment 07). It is inert test data — it was
written by the test author, for the test, and is labeled as such in the fixture
itself.

## Why fixtures matter to the methodology

The experiment's preregistered predictions (`exp07-prereg.md`) were
frozen *before* these fixtures were run through the gate. The raw results
(`exp07-results.json`) record what actually happened. Comparing the
two is the entire evaluation. Because the same author wrote the fixtures, the
predictions, and the gate, these results demonstrate self-consistency — not
blind accuracy. See the main README's honest-scoping section.
