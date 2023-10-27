# Test Scenario

#### Unique ID: POSdelete

**Description:** Test cases for the "Stop smeshing and delete PoS data" feature.

**Priority:** 1

**Prerequisites:** Smapp application is running, and PoS data is available for testing.

**Test Cases:**

[01](#test-case-id-POSdelete-01) - Confirm that the "Stop smeshing and delete PoS data" option is available after clicking the "Edit" button and all the buttons are responding as expected.

[02](#test-case-id-POSdelete-02) - Validate that clicking the "Delete Data" button stops the Smeshing process.

[03](#test-case-id-POSdelete-03) - Check that the PoS data is actually deleted after clicking "Delete Data".

[04](#test-case-id-POSdelete-04) - Verify that the user is redirected to the "Wallet" screen after the PoS data deletion process.

[05](#test-case-id-POSdelete-05) - Validate that the Smeshing screen is now reset and allows for new PoS Data setup.

[06](#test-case-id-POSdelete-06) - Confirm that there is a confirmation dialog before the actual deletion of PoS data.

[07](#test-case-id-POSdelete-07) - Verify the behavior when trying to delete PoS data while Smeshing is in an active state.

[08](#test-case-id-POSdelete-08) - Validate the behavior when trying to delete PoS data while Smeshing is in a paused or stopped state.

[09](#test-case-id-POSdelete-09) - Check that the PoS deletion action is logged or recorded in the application's logs.

[10](#test-case-id-POSdelete-10) - Confirm that the PoS data deletion does not affect other functionalities in the Wallet or Smeshing screens.

[11](#test-case-id-POSdelete-11) - Verify that the PoS data deletion does not affect wallet balance or transaction history.

[12](#test-case-id-POSdelete-12) - Validate the behavior when the user cancels the PoS data deletion process.

[13](#test-case-id-POSdelete-13) - Test the functionality with different types of PoS data (e.g., small, large, corrupted).

[14](#test-case-id-POSdelete-14) - Confirm that appropriate error messages are displayed if the deletion process fails for any reason.

[15](#test-case-id-POSdelete-15) - Verify the behavior when the Network connection is lost during the PoS data deletion process.

[16](#test-case-id-POSdelete-16) - Check the behavior on different platforms and operating systems to ensure consistency.

[17](#test-case-id-POSdelete-17) - Confirm that the UI elements and texts are displayed correctly during the whole process.

[18](#test-case-id-POSdelete-18) - Validate that PoS data deletion works correctly for different user roles or permission levels.

[19](#test-case-id-POSdelete-19) - Validate that the node successfully restarts after the PoS data is deleted.

[20](#test-case-id-POSdelete-20) - Confirm that all Smeshing-related processes are gracefully terminated before the node restarts.

[21](#test-case-id-POSdelete-21) - Check if the node restart triggers any unintended side effects in the Smeshing or Wallet screens.

[22](#test-case-id-POSdelete-22) - Verify that the user is informed or notified about the node restart.

[23](#test-case-id-POSdelete-23) - Validate if the node restart is logged or recorded in the application's history or logs.

[24](#test-case-id-POSdelete-24) - Verify the state of the Smeshing screen during the restart and immediately after the node restarts.

[25](#test-case-id-POSdelete-25) - Validate the behavior when the node fails to restart after PoS data deletion.

[26](#test-case-id-POSdelete-26) - Confirm that the system recovers gracefully if the node restart is interrupted or fails.

[27](#test-case-id-POSdelete-27) - Verify that the node restart does not affect the performance or stability of the Smapp application.

[28](#test-case-id-POSdelete-28) - Test if any Smeshing rewards collected before PoS data deletion are preserved after the node restarts (gRPC, balance in GUI, Explorer).

[29](#test-case-id-POSdelete-29) - Confirm that the PoS data deletion and node restart do not produce memory leaks or resource locking issues.

[30](#test-case-id-POSdelete-30) - Validate that the node restart occurs in a reasonable timeframe.

[31](#test-case-id-POSdelete-31) - Confirm that rollback mechanisms are in place in case the PoS data deletion or node restart fails.

[32](#test-case-id-POSdelete-32) - Validate the behavior if the user navigates away from the Smeshing screen during the PoS data deletion.

[33](#test-case-id-POSdelete-33) - Check how the feature behaves when executed during periods of high system load or CPU usage.

---

# Test Cases

#### Test Case ID: POSdelete-01

**Description:** Confirm that the "Stop smeshing and delete PoS data" option is available after clicking the "Edit" button and all the buttons are responding as expected.

**Steps:**

1. Open the Smapp application.
2. Navigate to the Smeshing screen.
3. Click the "Edit" button.
4. Check if the "Stop smeshing and delete PoS data" option is available.
5. Verify that all buttons on the screen respond as expected.

**Test Data:** None required.

**Expected Result:** The "Stop smeshing and delete PoS data" option is available, and all buttons respond as expected.

---

#### Test Case ID: POSdelete-02

**Description:** Validate that clicking the "Delete Data" button stops the Smeshing process.

**Steps:**

1. Open the Smapp application.
2. Navigate to the Smeshing screen.
3. Click the "Delete Data" button.
4. Confirm deletion.
5. Observe the Smeshing process.

**Test Data:** POS data linked in smapp

**Expected Result:** The Smeshing process stops after deleting POS

---

#### Test Case ID: POSdelete-03

**Description:** Check that the PoS data is actually deleted after clicking "Delete Data."

**Steps:**

1. Open the Smapp application.
2. Navigate to the Smeshing screen.
3. Click the "Delete Data" button.
4. Verify that PoS data is deleted.

**Test Data:**  POS data and directory

**Expected Result:** PoS data is deleted successfully after clicking "Delete Data."


---

#### Test Case ID: POSdelete-04

**Description:** Verify that the user is redirected to the "Wallet" screen after the PoS data deletion process.

**Steps:**

1. Open the Smapp application.
2. Navigate to the Smeshing screen.
3. Delete data
4. Observe the redirection.

**Test Data:** POS data

**Expected Result:** The user is redirected to the "Wallet" screen after the PoS data deletion process.


---

#### Test Case ID: POSdelete-05

**Description:** Validate that the Smeshing screen is now reset and allows for new PoS Data setup.

**Steps:**

1. Open the Smapp application.
2. Navigate to the Smeshing screen.
3. Delete data
4. Check if the Smeshing screen is reset.

**Test Data:** POS data

**Expected Result:** The Smeshing screen is reset and allows for new PoS Data setup.


---

# to be continued....

