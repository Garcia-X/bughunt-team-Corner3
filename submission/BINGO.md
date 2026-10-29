# Testing Bingo: Team Corner3

**Team captain:** Xavier Garcia
**Team members:** Xavier Garcia, Daniel Elias, Gabriel Elias

One person (the team captain) fills this in. Put the Test ID of a **failing** test case in each square you earn. One test case can only fill **one** square.

## The Card

| | | |
|:---:|:---:|:---:|
| **Unit**<br/>Test ID: XG-02 | **Integration**<br/>Test ID: | **System (E2E)**<br/>Test ID: |
| **Boundary Value**<br/>Test ID: XG-01 | **VALIDATION BUG**<br/>Test ID: | **Negative**<br/>Test ID: GE-01 |
| **Security**<br/>Test ID: DE-01 | **Acceptance**<br/>Test ID: | **Traced to a DIAGRAM**<br/>Test ID: |

The center square needs a test case labeled **Validation**. The bottom-right square needs a test case whose "Traces to" field names the architecture diagram, the class diagram, or the sequence diagram.

## Score Tally

| Item | How it scores | Count | Points |
|---|---|---:|---:|
| Unique failing test cases | 1 point each | 4 | 4 |
| Test types used (out of 7) | +2 points each | 4 | 8 |
| Validation bugs found | +3 points each | 0 | 0 |
| Any full row, column, or diagonal | +3 points each | 1 | 3 |
| Full card (blackout) | +5 points | 0 | 0 |
| **Total** | | | **15** |

**Rules for counting:**
- Two test cases that expose the **same bug** count as one.
- A test case only counts if it **fails** and has every field filled in.
- The instructor has the final say on what counts as a unique bug.

## Our Scariest Bug (for presentations)

**Test ID:** DE-01
**In one sentence, what is the bug?** A logged-out visitor can delete another user's costume from the Gallery.
**Verification or Validation, and why?** Verification—the app violates REQ-08, which allows only the costume owner to delete it.
