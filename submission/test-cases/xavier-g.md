# Test Cases: Xavier-G

**Team number:** Corner3

---

**Test ID:** XG-01
**Written by:** Xavier Garcia
**Title:** Registration accepts a password shorter than eight characters
**Traces to:** REQ-01
**Test type:** Boundary Value
**Preconditions:** On the Log In / Register page. The test username does not already exist in this browser's app data.
**Test data:** Username: `XG77`; password: `boo1234` (7 characters).

**Steps:**
1. Open the Log In / Register page.
2. Enter `XG77` in the Register username field.
3. Enter `boo1234` in the Register password field.
4. Click Create Account.

**Expected result:** Registration is rejected because the password has fewer than 8 characters. The app displays an error and does not create the account.
**Actual result:** The app displayed “Account created! You can log in now.”
**Status:** Fail
**Severity:** Major
**V or V:** Verification

---

**Test ID:** XG-02
**Written by:** Xavier Garcia
**Title:** Submission function accepts an empty costume description
**Traces to:** REQ-05
**Test type:** Unit
**Preconditions:** Logged in as `ghost_gary` with the Gallery open and browser Console available.
**Test data:** Name: `Blank Description Test`; description: empty string `""`; category: `Spooky`.

**Steps:**
1. Open the browser Console.
2. Enter `submitCostume("Blank Description Test", "", "Spooky")` and press Enter.
3. Find `Blank Description Test` in the Gallery.

**Expected result:** The function rejects the submission because a description is required. `Blank Description Test` does not appear in the Gallery.
**Actual result:** `Blank Description Test` appeared in the Gallery with no description and 0 votes.
**Status:** Fail
**Severity:** Major
**V or V:** Verification
