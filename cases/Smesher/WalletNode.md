# Test Scenario

#### Unique ID:  WalletNodeCreation

**Description:** Creation of Wallet+Node type of wallet

**Priority:** 1

**Prerequisites:** Smapp installed correctly, Internet connectivity

**Test Cases:**

[01](#test-case-id-walletnodecreation-01) - Validate successful wallet creation with all default settings

[02](#test-case-id-walletnodecreation-02) - Validate successful wallet creation choosing the 12-word mnemonic security level

[03](#test-case-id-walletnodecreation-03) - Validate successful wallet creation choosing the 24-word mnemonic security level

[04](#test-case-id-walletnodecreation-04) - Validate that typing an incorrect password the second time shows an error

[05](#test-case-id-walletnodecreation-05) - Validate wallet custom name input with valid characters

[06](#test-case-id-walletnodecreation-06) - Validate wallet custom name input with invalid characters

[07](#test-case-id-walletnodecreation-07) - Validate the wallet custom name maximum character limit (31 characters)

[08](#test-case-id-walletnodecreation-08) - Validate mnemonic backup setup

[09](#test-case-id-walletnodecreation-09) - Validate the ability to skip the mnemonic backup setup

[10](#test-case-id-walletnodecreation-10) - Validate that the correct network is selected and displayed

[11](#test-case-id-walletnodecreation-11) - Validate that the wallet overview screen is displayed after successful wallet creation

[12](#test-case-id-walletnodecreation-12) - Validate that the .json wallet file is created in the default Smapp directory

[13](#test-case-id-walletnodecreation-13) - Validate that the wallet custom name is used as the .json file name if provided

[14](#test-case-id-walletnodecreation-14) - Validate that the wallet custom name is displayed correctly in the app

[15](#test-case-id-walletnodecreation-15) - Validate that the network starts syncing after wallet creation

[16](#test-case-id-walletnodecreation-16) - Validate that the application is in local node mode and can set up smeshing

[17](#test-case-id-walletnodecreation-17) - Validate the display of confirmation screen with a link to the wallet file location and a "go to wallet" button

[18](#test-case-id-walletnodecreation-18) - Validate that the application handles a disconnection from the network during the setup process

[19](#test-case-id-walletnodecreation-19) - Validate error handling when trying to create a wallet with an already existing name

[20](#test-case-id-walletnodecreation-20) - Validate wallet creation while the application is undergoing a software update

[21](#test-case-id-walletnodecreation-21) - Validate that the "Back" button on each screen returns to the previous step without loss of already entered data

[22](#test-case-id-walletnodecreation-22) - Validate wallet creation on different operating systems (Windows, macOS, Linux)

[23](#test-case-id-walletnodecreation-23) - Validate UI responsiveness when creating a wallet on various screen resolutions

[24](#test-case-id-walletnodecreation-24) - Validate that tooltips or help messages are displayed correctly for each option

[25](#test-case-id-walletnodecreation-25) - Validate that all buttons, links, or interactive elements are corrects and accessible via keyboard navigation

[26](#test-case-id-walletnodecreation-26) - Validate that the application logs capture all the relevant information during the wallet creation

[27](#test-case-id-walletnodecreation-27) - Validate that the user can't proceed if the mnemonics are not confirmed correctly (if not skipped)

[28](#test-case-id-walletnodecreation-28) - Validate that third-party software (like antivirus programs) does not interfere with wallet creation

[29](#test-case-id-walletnodecreation-29) - Validate wallet creation after a sudden application restart or crash

[30](#test-case-id-walletnodecreation-30) - Validate that an error message is shown if the user tries to proceed without setting a password

---

# Test Cases

#### Test Case ID: WalletNodeCreation-01

**Description:** Validate successful wallet creation with all default settings

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Choose "Standard Wallet"
5. Choose any network and click "Next"
6. Choose any mnemonic security level
7. Type a correct password twice
8. Skip setting the custom name of the Wallet
9. Skip mnemonic backup setup
10. Click "Go to the Wallet"

**Test Data:** N/A

**Expected Result:**

* A valid .json wallet file is created in the default Smapp directory
* Smapp is opened on the wallet overview screen
* The network is connected and starts syncing
* Smapp is in the local node mode

---
