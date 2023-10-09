# Test Scenario

#### Unique ID: LogOut

**Description:** Testing the Log Out functionality in Spacemesh Application (Smapp).

**Priority:** 1

**Prerequisites:** 
- User should have the Smapp application installed
- User should be logged into an active wallet

**Test Cases:**

[01](#test-case-id-logout-01) - Log out using the lock icon on every screen

[02](#test-case-id-logout-02) - Log out from the settings

[03](#test-case-id-logout-03) - Validate UI and tooltips

[04](#test-case-id-logout-04) - Logout behavior when multiple wallets are logged in

_____

# Test Cases

#### Test Case ID: LogOut-01

**Description:** Log out using the lock icon on every screen

**Steps:**
1. Open the Smapp application.
2. Locate the lock icon on the top right corner.
3. Hover over the lock icon to see the tooltip.
4. Click on the lock icon.

**Test Data:** N/A

**Expected Result:** 
- Tooltip should display "log out"
- Upon clicking, the user should be immediately logged out.
- The node -if running- should run with no interruptions

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: LogOut-02

**Description:** Log out from the settings

**Steps:**
1. Open the Smapp application.
2. Navigate to settings (top right corner, gear wheel icon).
3. Locate the "Close Wallet" section.
4. Click on the “Logout” button.

**Test Data:** N/A

**Expected Result:** 
- Upon clicking the “Logout” button, the user should be immediately logged out.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: LogOut-03

**Description:** Validate UI and tooltips

**Steps:**
1. Open the Smapp application.
2. Hover over all log out options and validate tooltips.

**Test Data:** N/A

**Expected Result:** 
- Tooltips should be correct and informative.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: LogOut-04

**Description:** Logout behavior when multiple wallets are logged in

**Steps:**
1. Open the Smapp application.
2. Log in to multiple wallets.
3. Perform the logout operation from any screen or settings.

**Test Data:** N/A

**Expected Result:** 
- Validate if the user is logged out of all wallets


**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]
