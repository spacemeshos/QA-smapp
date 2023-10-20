# Test Scenario

#### Unique ID: Filerestore

**Description:** restore a wallet using the .json file

**Priority:** 2

**Prerequisites:** a valid wallet file, a non valid .json file, a wallet with the modified permissions

**Test Cases:** 

### Test Cases:

Restore Wallet from Settings Screen

[1](#test-case-id-filerestore-01) - Verify that clicking on the "restore wallet from the file" option in the Settings screen initiates the restoration process.

[2](#test-case-id-filerestore-02) - Validate that the wallet is successfully restored from a .json backup file located in the Documents directory when initiated from the Settings screen.

[3](#test-case-id-filerestore-03) - Validate that an appropriate error message is displayed if the restore process fails (e.g. wallet file inaccessible before the process is finished)

[4](#test-case-id-filerestore-04) - Verify that all wallet data and settings are intact after restoring from the Settings screen.

[5](#test-case-id-filerestore-05) - Verify that the restoration process initiated from the Settings screen can be canceled by the user.

Restore Wallet During New App Setup

[6](#test-case-id-filerestore-06) - Verify that clicking "open existing wallet" during the new app setup initiates the restoration process.

[7](#test-case-id-filerestore-07) - Validate that the wallet is successfully restored from a .json backup file located in the Documents directory when chosen during the new app setup.

[8](#test-case-id-filerestore-08) - Validate that an appropriate error message is displayed if the restore process fails during the new app setup (e.g. wallet file inaccessible before the process is finished).

[9](#test-case-id-filerestore-09) - Verify that all wallet data and settings are intact after restoring during the new app setup.

Restore Wallet While Canceling New Wallet Creation

[10](#test-case-id-filerestore-10) - Verify that clicking "already have a wallet? recover it" while canceling the new wallet creation initiates the restoration process.

[11](#test-case-id-filerestore-11) - Validate that the wallet is successfully restored from a .json backup file located in the Documents directory when this option is chosen.

[12](#test-case-id-filerestore-12) - Validate that an appropriate error message is displayed if the restore process fails in this scenario.

[13](#test-case-id-filerestore-13) - Verify that all wallet data and settings are intact after restoring in this scenario.

General Restore Functionality

[14](#test-case-id-filerestore-14) - Validate that the restore option is disabled if there is an active wallet session (i.e., a wallet is already open).

[15](#test-case-id-filerestore-15) - Validate that the restore process does not affect other app settings and data unrelated to the wallet being restored (e.g.Smeshing).

[16](#test-case-id-filerestore-16) - Verify that the restore functionality works correctly on all supported operating systems (Windows, macOS, Linux).

[17](#test-case-id-filerestore-17) - Validate the integrity of the restored wallet by comparing it to the original backup file.

[18](#test-case-id-filerestore-18) - Validate that the restored wallet is encrypted and requires the user's password to unlock.

[19](#test-case-id-filerestore-19) - Verify that the restore functionality works correctly for the wallet file located in a custom directory.

[20](#test-case-id-filerestore-20) - Verify that the proper error message is displayed in case of the insufficient wallet file permissions.

[21](#test-case-id-filerestore-21) - Verify that Smapp reacts correctly on uploading an invalid wallet file or any other .json file.

[22](#test-case-id-filerestore-22) - Verify that the user can cancle the restoring process in all the scenarios (settings, app setup and wallet creation canceled).


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



---