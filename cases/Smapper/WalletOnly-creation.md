# Test Scenario

 <!-- just roughly put together, to be improved with more detailed info -->

#### Unique ID:  WalletOnlyCreation

**Description:** Test cases for creating a "Wallet-Only" type wallet in Smapp.

**Priority:** 1

**Prerequisites:** Smapp must be properly installed and operational, stable Internet connection, 

**Test Cases:**

[01](#test-case-id-WalletOnlyCreation-01) - Validate successful creation of "Wallet-Only" with all recommended steps

[02](#test-case-id-WalletOnlyCreation-02) - Validate creation by skipping optional steps

[03](#test-case-id-WalletOnlyCreation-03) - Validate mnemonic security level choices

[04](#test-case-id-WalletOnlyCreation-04) - Validate password input

[05](#test-case-id-WalletOnlyCreation-05) - Validate custom wallet name input

[06](#test-case-id-WalletOnlyCreation-06) - Validate mnemonics backup process

[07](#test-case-id-WalletOnlyCreation-07) - Validate network connection and sync

[08](#test-case-id-WalletOnlyCreation-08) - Validate functionality post-creation

[09](#test-case-id-walletonlycreation-09) - Validate error messaging for unsuccessful network connection.

[10](#test-case-id-walletonlycreation-10) - Validate wallet file location and accessibility.

[11](#test-case-id-walletonlycreation-11) - Validate the ability to switch modes to run a local node after initial setup.

_____

# Test Cases

#### Test Case ID: WalletOnlyCreation-01

**Description:** Validate successful creation of "Wallet-Only" with all recommended steps.

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet only"
4. Choose "Standard Wallet"
5. Choose the network and click "Next"
6. Click "next" on the remote API selection screen
7. Choose the mnemonic security level (12 or 24 words)
8. Type a valid password twice
9. Put a custom name for your wallet
10. Complete the mnemonics backup process
11. Click "go to the wallet!" on the confirmation screen

**Test Data:** Passwords, custom wallet name, mnemonic words

**Expected Result:** All steps successfully complete, wallet overview screen opens, and all expected features are operational.



---

#### Test Case ID: WalletOnlyCreation-02

**Description:** Validate creation by skipping optional steps.

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet only"
4. Choose "Standard Wallet"
5. Choose the network and click "Next"
6. Click "next" on the remote API selection screen
7. Choose the mnemonic security level (12 or 24 words)
8. Type a valid password twice
9. Skip entering a custom name for your wallet
10. Skip the mnemonics backup process
11. Click "go to the wallet!" on the confirmation screen

**Test Data:** Passwords, no custom wallet name, no mnemonic words

**Expected Result:** Wallet is created and is functional but lacks a custom name and mnemonics backup.



---

#### Test Case ID: WalletOnlyCreation-03

**Description:** Validate mnemonic security level choices (12 or 24 words).

**Steps:**

1. Follow Steps 1-6 from Test Case ID: WalletOnlyCreation-01
2. Choose 12 words as mnemonic security level
3. Complete the rest of the steps
4. Repeat the process but choose 24 words as mnemonic security level

**Test Data:** 12 or 24 mnemonic words

**Expected Result:** Wallet is created successfully for both 12 and 24 mnemonic words.



---

#### Test Case ID: WalletOnlyCreation-04

see the [Password Setup scenario](cases/Smapper/Password-setup.md)

---

#### Test Case ID: WalletOnlyCreation-05

**Description:** Validate custom wallet name input.

**Steps:**

1. Follow Steps 1-8 from Test Case ID: WalletOnlyCreation-01
2. Enter a custom wallet name containing special characters
3. Attempt to proceed

**Test Data:** Custom wallet name with special characters

**Expected Result:** System either accepts the name or shows an appropriate error message.



---

#### Test Case ID: WalletOnlyCreation-06

**Description:** Validate mnemonics backup process.

**Steps:**

1. Follow Steps 1-8 from Test Case ID: WalletOnlyCreation-01
2. Complete mnemonics backup by dragging and dropping 4 random words in incorrect places
3. Attempt to proceed

**Test Data:** Incorrect mnemonic words

**Expected Result:** System prevents proceeding and shows an error message.



---

#### Test Case ID: WalletOnlyCreation-07

**Description:** Validate network connection and sync.

**Steps:**

1. Complete wallet creation successfully
2. Observe the network status

**Test Data:** None

**Expected Result:** The network is connected and synced instantly.



---

#### Test Case ID: WalletOnlyCreation-08

**Description:** Validate functionality post-creation.

**Steps:**

1. Complete wallet creation successfully
2. Attempt to execute transactions (send some SMH on this address in a first place)

**Test Data:** Transaction details

**Expected Result:** Transactions can be executed without syncing network data or running a full node.



---

#### Test Case ID: WalletOnlyCreation-09

**Description:** Validate error messaging for unsuccessful network connection.

**Steps:**

1. Disable network connectivity on the testing machine.
2. Attempt to create a "Wallet-Only" type wallet.
  
**Test Data:** None

**Expected Result:** An appropriate error message indicating the network issue should be displayed.



---

#### Test Case ID: WalletOnlyCreation-10

**Description:** Validate wallet file location and accessibility.

**Steps:**

1. Complete wallet creation successfully.
2. Visit the file location as indicated on the confirmation screen.
  
**Test Data:** File path

**Expected Result:** The wallet file should be present at the indicated location and should be accessible.



---

#### Test Case ID: WalletOnlyCreation-11

**Description:** Validate the ability to switch modes to run a local node after initial setup.

**Steps:**

1. Complete wallet creation for "Wallet-Only" type.
2. Navigate to settings to switch to running a local node.
  
**Test Data:** None

**Expected Result:** Switching to local node should be successful and operational.



---



