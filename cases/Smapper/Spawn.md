# Test Scenario

#### Unique ID:  Spawn

**Description:** Test cases for the "Spawn" transaction feature in Smapp.

**Priority:** 1

**Prerequisites:** Smapp must be properly installed, operational, and synced. A newly created Wallet must be present.

**Test Cases:**

[01](#test-case-id-Spawn-01) - Validate the availability of the "Spawn" button for a newly created Wallet

[02](#test-case-id-Spawn-02) - Validate the self-spawn transaction window

[03](#test-case-id-Spawn-03) - Validate unlocking of the Send SMH option

[04](#test-case-id-Spawn-04) - Validate error handling during Spawn transaction

[05](#test-case-id-Spawn-05) - Validate timeout handling 

[06](#test-case-id-Spawn-06) - Validate the transaction log entry for self-spawn

[07](#test-case-id-Spawn-07) - Validate the UI/UX elements during the Spawn transaction

[08](#test-case-id-Spawn-08) - Validate behavior during network disruptions

[09](#test-case-id-Spawn-09) - Validate resource utilization 

[10](#test-case-id-Spawn-10) - Validate logs and auditing  

_____

# Test Cases

#### Test Case ID: Spawn-01

**Description:** Validate the availability of the "Spawn" button for a newly created Wallet.

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen

**Test Data:** None

**Expected Result:** The "Spawn" button should be visible and available for a newly created Wallet.



---

#### Test Case ID: Spawn-02

**Description:** Validate the self-spawn transaction window.

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen
3. Click the "Spawn" button

**Test Data:** None

**Expected Result:** The self-spawn transaction window should appear showing correct Account details and fees options.



---

#### Test Case ID: Spawn-03

**Description:** Validate unlocking of the Send SMH option.

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen
3. Successfully submit the spawn transaction

**Test Data:** None

**Expected Result:** The Send SMH option should be unlocked and fully functional.



---

#### Test Case ID: Spawn-04

**Description:** Validate error handling during Spawn transaction

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen
3. Attempt a Spawn transaction that should fail (e.g., insufficient balance, server error)

**Test Data:** None

**Expected Result:** Proper error messages should be displayed to guide the user.



---

#### Test Case ID: Spawn-05

**Description:** Validate timeout handling.

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen and sucessfully sumbit Spawn tx. 
3. Wait until the transaction is completed, note how much time has passed.
4. Check what happens after 3, 5 and 10 minutes, if the transaction is applied and you are able to submit a regular tx.

**Test Data:** None

**Expected Result:** The spawn transactions should be applied. The Spawn button should be greyed out during the tx processing. After the tx is submitted, the Spawn button should disappear, we should see the Send button.


---

#### Test Case ID: Spawn-06

**Description:** Validate the transaction log entry for self-spawn.

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen
3. Successfully submit the spawn transaction
4. Go to the transaction log

**Test Data:** None

**Expected Result:** The self-spawn transaction should exist in the transaction log with all details.



---

#### Test Case ID: Spawn-07

**Description:** Validate the UI/UX elements during the Spawn transaction.

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen
3. Observe UI elements and UX design involved in the Spawn transaction

**Test Data:** None

**Expected Result:** All UI/UX elements should be responsive and clear.



---

#### Test Case ID: Spawn-08

**Description:** Validate behavior during network disruptions.

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen
3. Initiate a Spawn transaction
4. Disconnect from the network during the transaction

**Test Data:** None

**Expected Result:** The application should display an appropriate error or warning message, the tx should be correctly applied once the Internet connection reestablished and node is synced. The tx should not be applied if the node isn't synced, it should not be frozen in the pending or any other state. 



---

#### Test Case ID: Spawn-09

**Description:** Validate resource utilization during the Spawn transaction.

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen
3. Monitor CPU and memory usage during the Spawn transaction

**Test Data:** None

**Expected Result:** CPU and memory utilization should remain within acceptable limits.



---

#### Test Case ID: Spawn-10

**Description:** Validate logs and auditing for the Spawn transaction.

**Steps:**

1. Open Smapp
2. Go to the "Wallet" screen
3. Initiate a Spawn transaction
4. Check app-logs and go-spacemesh log files

**Test Data:** None

**Expected Result:** All actions should be correctly logged for auditing purposes.



---


