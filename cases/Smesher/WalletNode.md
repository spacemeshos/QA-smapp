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

[19](#test-case-id-walletnodecreation-19) - Validate trying to create a wallet with an already existing name

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

#### Test Case ID: WalletNodeCreation-02

**Description:** Validate successful wallet creation choosing the 12-word mnemonic security level

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Choose "Standard Wallet"
5. Choose the network and click "Next"
6. Choose the 12-word mnemonic security level
7. Type a password twice
8. Skip setting the custom name of the Wallet
9. Skip mnemonic backup setup
10. Click "Finish"

**Test Data:** N/A

**Expected Result:**

* A valid .json wallet file is created in the default Smapp directory
* Smapp is opened on the wallet overview screen
* The network is connected and starts syncing
* Smapp is in the local node mode
* No issues with the backup process or general wallet use

---

#### Test Case ID: WalletNodeCreation-03

**Description:** Validate successful wallet creation choosing the 24-word mnemonic security level

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Choose "Standard Wallet"
5. Choose the network and click "Next"
6. Choose the 24-word mnemonic security level
7. Type a password twice
8. Skip setting the custom name of the Wallet
9. Skip mnemonic backup setup
10. Click "Finish"

**Test Data:** N/A

**Expected Result:**

* A valid .json wallet file is created in the default Smapp directory
* Smapp is opened on the wallet overview screen
* The network is connected and starts syncing
* Smapp is in the local node mode
* No issues with the backup process or general wallet use

---

#### Test Case ID: WalletNodeCreation-04

**Description:** Validate that typing an incorrect password the second time shows an error

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Type a password in the first field
5. Type a different password in the second field
6. Attempt to proceed to the next step

**Test Data:** First password: "password1", Second password: "password2"

**Expected Result:**

* An error message is displayed stating the passwords do not match

---

#### Test Case ID: WalletNodeCreation-05

**Description:** Validate wallet custom name input with valid characters

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Enter a custom name for the wallet using valid characters (latin letters, numbers, underscore, and hyphen)
5. Complete the remaining steps to create the wallet

**Test Data:** Wallet name: "My_Wallet-123"

**Expected Result:**

* The custom name is used as the wallet name in the application and as the .json file name

---

#### Test Case ID: WalletNodeCreation-06

**Description:** Validate wallet custom name input with invalid characters

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Enter a custom name for the wallet using invalid characters (e.g., special characters like @, #, etc.)
5. Attempt to proceed to the next step

**Test Data:** Wallet name: "My@Wallet#"

**Expected Result:**

* An error message is displayed stating that the characters are invalid

---

#### Test Case ID: WalletNodeCreation-07

**Description:** Validate the wallet custom name maximum character limit

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Enter a custom name for the wallet with more than 31 characters
5. Complete the remaining steps to create the wallet

**Test Data:** Wallet name: "MyVeeeryLongWalletNameWith31Chars"

**Expected Result:**

* The custom name with more than 31 characters is not accepted and not used as the wallet name in the application or as the .json file name

---

#### Test Case ID: WalletNodeCreation-08

**Description:** Validate mnemonic backup setup (more on this in the mnemonics test scenarios)

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Complete all steps up to mnemonic backup
5. Set up the mnemonics backup by confirming the mnemonics
6. Complete the wallet creation process

**Test Data:** Mnemonics provided by the app

**Expected Result:**

* The mnemonics are backed up and the wallet is created successfully

---

#### Test Case ID: WalletNodeCreation-09

**Description:** Validate the ability to skip the mnemonic backup setup even if started

**.Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Start the mnemonics backup process
5. Go back and click the "Skip" button
6. Complete the wallet creation process

**Test Data:** N/A

**Expected Result:**

* The wallet is created successfully without setting up mnemonic backup

---

#### Test Case ID: WalletNodeCreation-10

**Description:** Validate that the correct network is selected and displayed

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Choose the network (e.g., Mainnet, Testnet)
5. Complete the wallet creation process

**Test Data:** Selected network (Mainnet/Testnet)

**Expected Result:**

* The selected network is displayed and connected (Network screen) )after the wallet is created
* THis network is set once the wallet is opened, even if we use another wallet with a different network in the same app.
* The User should be able to switch the network anytime.

---

#### Test Case ID: WalletNodeCreation-11

**Description:** Validate that the wallet overview screen is displayed correctly after successful wallet creation

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Complete the wallet creation process
5. Click "Finish"

**Test Data:** N/A

**Expected Result:**

* The wallet overview screen is displayed with the correct balance (0SMH), Wallet name (default or custom)
* there are no GUI or functional issues

---

#### Test Case ID: WalletNodeCreation-12

**Description:** Validate that the .json wallet file is created in the default Smapp (installation) directory

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Complete the wallet creation process
5. Click "Finish"
6. Navigate to the default Smapp directory to check for the .json wallet file

**Test Data:** Default Smapp directory location

**Expected Result:**

* A .json wallet file is present in the default Smapp directory

---

#### Test Case ID: WalletNodeCreation-13

**Description:** Validate that the wallet custom name is used as the .json file name if provided

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Enter a custom name for the wallet
5. Complete the wallet creation process
6. Navigate to the default Smapp directory to check for the .json wallet file

**Test Data:** Wallet name: "My_Custom_Wallet"

**Expected Result:**

* A .json file with the custom name "My_Custom_Wallet(+the defaultopart of the name).json" is present in the default Smapp directory

---

#### Test Case ID: WalletNodeCreation-14

**Description:** Validate that the wallet custom name is displayed correctly in the app

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Enter a custom name for the wallet
5. Complete the wallet creation process

**Test Data:** Wallet name: "My_Custom_Wallet"

**Expected Result:**

* The custom name "My_Custom_Wallet" is displayed in the wallet overview screen

---

#### Test Case ID: WalletNodeCreation-15

**Description:** Validate that the network starts syncing after wallet creation

**Steps:**

1. Open Smapp (new node)
2. Click "Create"
3. Choose "Wallet+Node"
4. Complete the wallet creation process
5. Observe the network status

**Test Data:** N/A

**Expected Result:**

* The network is connected and starts syncing (it should not be synced immediately)
* The go-spacemesh process should be running (Activity monitor/task manager)
* The resources usage should not bew excessive

---

#### Test Case ID: WalletNodeCreation-16

**Description:** Validate that the application is in local node mode and can set up smeshing

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Complete the wallet creation process
5. Go to the Smeshing screen and check if you can set up Smeshing

**Test Data:** N/A

**Expected Result:**

* The application is in local node mode and allows for smeshing setup

---

#### Test Case ID: WalletNodeCreation-17

**Description:** Validate the display of confirmation screen with a link to the wallet file location

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Complete the wallet creation process
5. click the wallet location linlk on the confirmation screen

**Test Data:** N/A

**Expected Result:**

* A confirmation screen appears displaying a link to the wallet file location
* The link leads to the correct wallet file

---

#### Test Case ID: WalletNodeCreation-18

**Description:** Validate that the application handles a disconnection from the network during the setup process

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Disconnect the internet during the setup process
5. Observe the setup process in smapp
6. Switch the Internet back on

**Test Data:** N/A

**Expected Result:**

* An error message is displayed
* There's not Network available to choose
* User cannot proceed with the wallet creation
* After the Internet is back, the User should be able to resume setup process with no issues.

---


#### Test Case ID: WalletNodeCreation-19

**Description:** Validate] trying to create a wallet with an already existing name

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Enter a custom name that already exists in the app for another wallet
5. Complete the wallet creation process

**Test Data:** Wallet name: "Existing_Wallet_Name"

**Expected Result:**

* there's no error, User is able to generate many Wallets with the same custom name
* the .json file wallet name contains a part with a creation date&time



---

#### Test Case ID: WalletNodeCreation-20

**Description:** Validate wallet creation while the application is undergoing a software update

**Steps:**

1. Start a software update for Smapp
2. During the update, attempt to create a new wallet

**Test Data:** N/A

**Expected Result:**

* The wallet creation process is either successfully completed or an appropriate error message is displayed



---

#### Test Case ID: WalletNodeCreation-21

**Description:** Validate that the "Back" button on each screen returns to the previous step without loss of already entered data

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Enter some data and navigate to the next step
5. Click the "Back" button

**Test Data:** Any valid wallet creation data

**Expected Result:**

* The application returns to the previous screen and retains all previously entered data



---

#### Test Case ID: WalletNodeCreation-22

**Description:** Validate wallet creation on different operating systems (Windows, macOS, Linux)

**Steps:**

1. Open Smapp on Windows
2. Create a new wallet following the standard procedure
3. Repeat steps 1 and 2 on macOS and Linux

**Test Data:** N/A

**Expected Result:**

* Wallet creation is successful on all three operating systems



---

#### Test Case ID: WalletNodeCreation-23

**Description:** Validate UI responsiveness when creating a wallet on various screen resolutions

**Steps:**

1. Change your display settings to a low resolution
2. Open Smapp
3. Click "Create"
4. Choose "Wallet+Node"
5. Complete the wallet creation process
6. Repeat the process for medium and high resolutions

**Test Data:** Screen resolutions - low, medium, high

**Expected Result:**

* The UI adapts appropriately to each screen resolution, and the wallet creation process can be completed without issues



---

#### Test Case ID: WalletNodeCreation-24

**Description:** Validate that tooltips or help messages are displayed correctly for each option

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Hover over tooltips or click on help icons

**Test Data:** N/A

**Expected Result:**

* Tooltips and help messages are displayed correctly and provide relevant information



---

#### Test Case ID: WalletNodeCreation-25

**Description:** Validate that all buttons, links, or interactive elements are correct and accessible via keyboard navigation

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Use the keyboard to navigate through all interactive elements

**Test Data:** N/A

**Expected Result:**

* All interactive elements are navigable via keyboard and function as expected



---

#### Test Case ID: WalletNodeCreation-26

**Description:** Validate that the application logs capture all the relevant information during the wallet creation

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Complete the wallet creation process
5. Check the application logs

**Test Data:** N/A

**Expected Result:**

* All relevant actions and events during wallet creation are logged



---

#### Test Case ID: WalletNodeCreation-27

**Description:** Validate that the user can't proceed if the mnemonics are not confirmed correctly (if not skipped)

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. When prompted to confirm mnemonics, enter incorrect mnemonics

**Test Data:** Incorrect mnemonics

**Expected Result:**

* The user is not allowed to proceed and an error message is displayed



---

#### Test Case ID: WalletNodeCreation-28

**Description:** Validate that third-party software (like antivirus programs) does not interfere with wallet creation

**Steps:**

1. Install a third-party antivirus program
2. Open Smapp
3. Click "Create"
4. Choose "Wallet+Node"
5. Complete the wallet creation process

**Test Data:** N/A

**Expected Result:**

* Wallet creation is not interfered with by third-party software



---

#### Test Case ID: WalletNodeCreation-29

**Description:** Validate wallet creation after a sudden application restart or crash

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Force quit Smapp or induce a crash
5. Restart Smapp and attempt to resume the wallet creation process

**Test Data:** N/A

**Expected Result:**

* An appropriate error message is displayed or the user is allowed to resume wallet creation



---

#### Test Case ID: WalletNodeCreation-30

**Description:** Validate that an error message is shown if the user tries to proceed without setting a password

**Steps:**

1. Open Smapp
2. Click "Create"
3. Choose "Wallet+Node"
4. Skip the password setup and try to proceed

**Test Data:** N/A

**Expected Result:**

* An error message is displayed, indicating that setting a password is mandatory


