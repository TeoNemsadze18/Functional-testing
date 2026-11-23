# AUTH-BTN-001 – Tapping "Continue" Automatically Triggers "Forget Password"

* **Severity:** High
* **Environment:** Mobile App (Android 14 · Staging · v1.21.0)
* **Reproducibility:** 100%

## Summary
On the authentication screen, after entering an email address and tapping the "Continue" button, the "Forget password" button is automatically triggered at the same time. Repeatedly tapping "Continue" reproduces this behavior every time.

## Steps
1. Open the authentication screen.
2. Tap "Continue to email".
3. Enter a valid email address.
4. Tap the "Continue" button.
5. Repeat tapping "Continue" and observe the behavior of the "Forget password" button.

## Actual
Each tap on the "Continue" button automatically triggers/activates the "Forget password" button as well.

## Expected
Tapping "Continue" should execute only the email submission/continuation action. "Forget password" should trigger only when explicitly tapped by the user.

## Notes
Subcategory: Functional Correctness. Likely overlapping touch/hit areas or unintended click event propagation between adjacent authentication controls.
