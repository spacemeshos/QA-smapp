# Test Scenario

#### Unique ID:  Autostart

**Description:** Testing the "Autostart" feature in Smapp.

**Priority:** 2

**Prerequisites:** Smapp must be properly installed and operational.

**Test Cases:**

[01](#test-case-id-Autostart-01) - Validate the presence of the "autostart" option

[02](#test-case-id-Autostart-02) - Validate the functionality of toggling "ON"

[03](#test-case-id-Autostart-03) - Validate the functionality of toggling "OFF"

[04](#test-case-id-Autostart-04) - Validate the setting persistence after application restart

[05](#test-case-id-Autostart-05) - Validate the system permission dialog (if applicable)

[06](#test-case-id-Autostart-06) - Validate the "Autostart" setting after reinstalling the app

[07](#test-case-id-Autostart-07) - Validate the "Autostart" setting after updating the app

_____

# Test Cases

#### Test Case ID: Autostart-01

**Description:** Validate the presence of the "autostart" option.

**Steps:**

1. Open Smapp
2. Go to settings via the gear wheel icon
3. Navigate to the Wallet section

**Test Data:** None

**Expected Result:** The "autostart" option should be visible.



---

#### Test Case ID: Autostart-02

**Description:** Validate the functionality of toggling "ON".

**Steps:**

1. Follow Steps 1-3 from Test Case ID: Autostart-01
2. Click “Toggle autostart”
3. Restart your PC
4. Ccheck the Smapp status (open or not), and the processes in Task Manager/Activity Monitor

**Test Data:** None

**Expected Result:** 
- The "OFF/ON" part of the settings explanatory phrase should change to "ON".
- The app should autostart on system startup
- go-spacemesh and other processes should be launched automatically


--- 

#### Test Case ID: Autostart-03

**Description:** Validate the functionality of toggling "OFF".

**Steps:**

1. Follow Steps 1-3 from Test Case ID: Autostart-01
2. If "Toggle autostart" is "ON", click to toggle it "OFF"
3. Restart PC
4. Check the Smapp status (open or not), and the processes in Task Manager/Activity Monitor
**Test Data:** None

**Expected Result:** 
- The "OFF/ON" part of the settings explanatory phrase should change to "OFF".
- The app should NOT autostart on system startup
- go-spacemesh and other processes should NOT be launched automatically


---

#### Test Case ID: Autostart-04

**Description:** Validate the setting persistence after application restart.

**Steps:**

1. Follow Steps 1-3 from Test Case ID: Autostart-01
2. Toggle the "autostart" option to "ON"
3. Close Smapp and reopen it
4. Go back to the Wallet section in settings

**Test Data:** None

**Expected Result:** The "Wallet auto start" setting should remain "ON" after restarting the application.



---

#### Test Case ID: Autostart-05

**Description:** Validate the system permission dialog (if applicable).

**Steps:**

1. Follow Steps 1-3 from Test Case ID: Autostart-01
2. Toggle the "autostart" option to "ON"

**Test Data:** None

**Expected Result:** A dialog window for system permissions may appear, depending on the system type and preferences.



---

#### Test Case ID: Autostart-06

**Description:** Validate the "Autostart" setting after reinstalling the app.

**Steps:**

1. Ensure the "Autostart" feature is enabled.
2. Uninstall Smapp. Don't delete any directories manually.
3. Reinstall Smapp.
4. Go to settings via the gear wheel icon in the upper right corner.
5. Navigate to the Wallet section.
6. Verify whether the "Autostart" setting is retained or reset after reinstalling the app.

**Test Data:** None

**Expected Result:**  The setting state should be kept.



---

#### Test Case ID: Autostart-07

**Description:** Validate the "Autostart" setting after updating the app.

**Steps:**

1. Ensure the "Autostart" feature is enabled.
2. Update Smapp to a newer version.
3. Go to settings via the gear wheel icon in the upper right corner.
4. Navigate to the Wallet section.

**Test Data:** None

**Expected Result:** The "Autostart" setting should be retained after updating the app.



---


