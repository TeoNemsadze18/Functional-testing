# LIVE-VOT-001 - Voting Round Timer Disappears After Moderator Rejoins

* **Severity:** Medium
* **Environment:** Android 14 · Red Note 14S · Staging · v1.23.0
* **Reproducibility:** 80%

## Summary
After a debate ends and the 30-second voting round begins, if the moderator leaves the live session and rejoins a few seconds later, the voting round remains active on screen, but the countdown timer disappears completely.

## Preconditions
User is in a live session as a moderator in the host format.

## Steps
1. Select or start the voting round.
2. Leave the live session.
3. Rejoin the live session after a few seconds and observe the voting screen.

## Actual
The voting round is visually shown, but the timer has disappeared and the remaining time is no longer displayed.

## Expected
Immediately upon the moderator rejoining, the active voting timer (remaining seconds) should be visible and continue counting down normally.

## Notes
Subcategory: Functional Correctness / Completeness. Timer state or UI binding is not properly restored upon rejoining an active voting round (80% reproducibility).
