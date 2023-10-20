# Test Scenario

#### Unique ID: Filebackup

**Description:** Backup wallet to the file from the Wallet overview screen and Settings.

**Priority:** 2

**Prerequisites:** 

**Test Cases:** 

Wallet Backup from Wallet Overview Screen

[1](#test-case-id-filebackup-01) - Verify that clicking on the backup option from the Wallet overview screen initiates the backup process.

[2](#test-case-id-filebackup-02) - Validate that a .json backup file is generated in the Documents directory after backup from the Wallet overview screen.

[3](#test-case-id-filebackup-03) - Validate that an appropriate error message is displayed if the backup fails from the Wallet overview screen.

[4](#test-case-id-filebackup-04) - Verify that the generated .json backup file can be successfully used to restore the wallet.

[5](#test-case-id-filebackup-05) - Verify that a backup initiated from the Wallet overview screen can be canceled by the user.

Wallet Backup from Settings Screen

[6](#test-case-id-filebackup-06) - Verify that clicking on the backup option from the Settings screen initiates the backup process.

[7](#test-case-id-filebackup-07) - Validate that a .json backup file is generated in the Documents directory after backup from the Settings screen.

[8](#test-case-id-filebackup-08) - Validate that an appropriate error message is displayed if the backup fails from the Settings screen.

[9](#test-case-id-filebackup-09) - Verify that the generated .json backup file can be successfully used to restore the wallet.

[10](#test-case-id-filebackup-10) - Verify that a backup initiated from the Settings screen can be canceled by the user.

General Backup Functionality

[11](#test-case-id-filebackup-11) - Validate that the backup button persists on the Wallet overview screen even after using this option succesfully. 

[12](#test-case-id-filebackup-12) - Validate that the backup process does not affect the wallet's existing data and settings.

[13](#test-case-id-filebackup-13) - Verify that an appropriate success message or notification is displayed once the backup is successful.

[14](#test-case-id-filebackup-14) - alidate that the backup file is encrypted and requires the user's password to restore.

[15](#test-case-id-filebackup-15) - Validate the backup functionality with insufficient disk space.

[16](#test-case-id-filebackup-16) - Validate the backup process with insufficient permissions to the default Documents directory.

[17](#test-case-id-filebackup-17) - Validate the backup process with custom wallet name.

[18](#test-case-id-filebackup-18) - Validate that older backup files are not overwritten.

[19](#test-case-id-filebackup-19) - Verify that a backup can be initiated while the wallet is performing other actions (e.g., a transaction).

[20](#test-case-id-filebackup-20) - Verify that backup functionality work correctly on all supported operating systems (Windows, macOS, Linux).



_____

# Test Cases

#### Test Case ID: 

**Description:**

**Steps:**

1. 

2. 

3. 

**Test Data:**

**Expected Result:**


