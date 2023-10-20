# Test Scenario

#### Unique ID: Install

**Description:** Smapp installation process from 0 to running app

**Priority:** 1

**Prerequisites:** Internet connection, minimal system requirements met, Visual C++ Redistributable, OpenCl support

**Test Cases:**

[01](#test-case-id-install-01) - Getting the right package

[02](#test-case-id-install-02) - Checking the package security - Virustotal scan and checksum verification (currently for go-spacemesh only)

[03](#test-case-id-install-03) - Default installation process on Mac 

[04](#test-case-id-install-04) - Default installation process on Windows

[05](#test-case-id-install-05) - Default installation process on Linux (AppImage)

[06](#test-case-id-install-06) - Default installation process on Linux (.deb )

[07](#test-case-id-install-07) - Custom directory on Windows for installation

[08](#test-case-id-install-08) - Custom permissions on Windows (for other users)

[09](#test-case-id-install-09) - Getting the unofficial package (prerelease, custom build etc.) and trying to install it on Mac

[10](#test-case-id-install-10) - Getting the unofficial package (prerelease, custom build etc.) and trying to install it on Windows

[11](#test-case-id-install-11) - Getting the unofficial package (prerelease, custom build etc.) and trying to install it on Ubuntu

[12](#test-case-id-install-12) - Installing and running Smapp on Windows without Visual C++ Redistributable

[13](#test-case-id-install-13) - Installing and running Smapp on Windows without OpenCl support

[14](#test-case-id-install-14) - Installing and running Smapp on Ubuntu without OpenCl support

[15](#test-case-id-install-15) - Running Smapp via CLI with flags - macOS

[16](#test-case-id-install-16) - Running Smapp via CLI with flags - Windows

[17](#test-case-id-install-17) - Running Smapp via CLI with flags - Ubuntu

[18](#test-case-id-Install-18) - Verify rollback functionality if installation fails on Windows

[19](#test-case-id-Install-19) - Verify rollback functionality if installation fails on Mac

[20](#test-case-id-Install-20) - Verify rollback functionality if installation fails on Linux

[21](#test-case-id-Install-21) - Verify Smapp behavior when disk space is insufficient for installation

[22](#test-case-id-Install-22) - Installation over an older version of Smapp without uninstalling the old version - Windows

[23](#test-case-id-Install-23) - Installation over an older version of Smapp without uninstalling the old version - Mac

[24](#test-case-id-Install-24) - Installation over an older version of Smapp without uninstalling the old version - Linux

[25](#test-case-id-Install-25) - Verify the installer's digital signature on Windows

[26](#test-case-id-Install-26) - Verify the installer's digital signature on Mac

[27](#test-case-id-Install-27) - Verify that Smapp auto-updates to a new version

[28](#test-case-id-Install-28) - Verify Smapp's firewall rules on Windows

[29](#test-case-id-Install-29) - Verify that Smapp doesn't affect system boot time

[30](#test-case-id-Install-30) - Validate Smapp’s data folder structure post-installation

[31](#test-case-id-Install-31) - Verify behavior when trying to install Smapp without admin rights

[32](#test-case-id-Install-32) - Installing Smapp when an antivirus program is running

[33](#test-case-id-Install-33) - Verify (in the task manager or activity monitor) the processes and resources usage

[34](#test-case-id-Install-34) - Validate that all installation logs are created and stored correctly

[35](#test-case-id-Install-35) - Verify the installation process in different languages (if applicable need to check it actually)

[36](#test-case-id-Install-36) - Verify that all Smapp services start correctly post-installation

[37](#test-case-id-Install-37) - Verify error handling for corrupted installation files

[38](#test-case-id-Install-38) - Verify network configurations - Smapp installation involves internet-based setups

[39](#test-case-id-Install-39) - Verify that Smapp does not overwrite user-customized settings when updating to a newer version

[40](#test-case-id-Install-40) - Verify that Smapp can be successfully uninstalled





_____

# Test Cases

#### Test Case ID: Install-01

**Description:** Getting the right package

**Steps:**

1. Go to the Spacemesh Github repository and open the Smapp repo (currently: https://github.com/spacemeshos/smapp) 

    1. Check the "Releases" section on the right side

    1. Open the '"latest"' release page

    1. Check the semantic version in the page header and in all the builds

    1. Check if all the links work and allow to download correctly the corresponding resource

1. Go to the Spacemesh official website and navigate to the page with the Smapp installers (currently: https://spacemesh.io/start/)

    1. Check the semver of the packages under the links

    1. Check if all the links work and allow to download correctly the corresponding resource

1. Go to the Spacemesh official Discord server and navigate to the channel with the Smapp update info and installers (currently: https://discord.com/channels/623195163510046732/691258865861394432)

    1. Check the semver of the packages under the links

    1. Check if all the links work and allow to download correctly the corresponding resource

1. Go to the Spacemesh official Twitter / X and find the post with the Smapp update info and installers (currently: https://x.com/teamspacemesh?s=20)

    1. Check the semver of the packages under the links

    1. Check if all the links work and allow to download correctly the corresponding resource



**Test Data:**

**Expected Result:**

- Smapp repository should exist within official Spacemesh GitHub resources
- The right release should be marked as 'latest' and visible in the Releases from the repo code view - central right side
- Semantic Version should be correct in all the artifacts (GitHub, Website, Discord, Twitter)
- All the links should lead to the latest Smapp release
- All the packages should be easily and correctly downloaded

**Actual Result:**

**Status:** Pass / Fail

---

#### Test Case ID: Install-02

**Description:** Verify that the go-spacemesh package is secure using a Virustotal scan and checksum verification.

**Steps:**

1. Download the go-spacemesh package.

2. Upload the package to Virustotal and await the scan results.

3. Compare the package checksum with the published checksum.

**Test Data:** go-spacemesh package

**Expected Result:** 

- Virustotal reports no threats.
- Checksums match.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-03

**Description:** Verify that Smapp can be installed successfully on a Mac using the default installation process.

**Steps:**

1. Download the Smapp Mac installer.

2. Run the installer.

3. Follow the installation prompts.

**Test Data:** Smapp Mac installer

**Expected Result:** 

- Installation is successful.
- Smapp launches automatically or manually without errors.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-04

**Description:** Verify that Smapp can be installed successfully on a Windows machine using the default installation process.

**Steps:**

1. Download the Smapp Windows installer.

2. Run the installer.

3. Follow the installation prompts.

**Test Data:** Smapp Windows installer

**Expected Result:** 

- Installation is successful.
- Smapp launches automatically or manually without errors.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-05

**Description:** Verify that Smapp can be installed successfully on a Linux machine using the AppImage.

**Steps:**

1. Download the Smapp AppImage for Linux.

2. Make the AppImage executable.

3. Run the AppImage.

**Test Data:** Smapp AppImage

**Expected Result:** 

- Installation is successful.
- Smapp launches automatically or manually without errors.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-06

**Description:** Verify that Smapp can be installed successfully on a Linux machine using the .deb package.

**Steps:**

1. Download the Smapp .deb package for Linux.

2. Install the .deb package using dpkg or apt.

3. Run Smapp.

**Test Data:** Smapp .deb package

**Expected Result:** 

- Installation is successful.
- Smapp launches automatically or manually without errors.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-07

**Description:** Verify that Smapp can be installed in a custom directory on Windows.

**Steps:**

1. Download the Smapp Windows installer.

2. Run the installer.

3. Choose a custom directory during the installation prompts.

**Test Data:** Smapp Windows installer, Custom directory path

**Expected Result:** 

- Installation is successful in the custom directory.
- Smapp launches automatically or manually without errors.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-08

**Description:** Verify that Smapp can be installed with custom permissions for other users on Windows.

**Steps:**

1. Download the Smapp Windows installer.

2. Run the installer as an administrator.

3. Set custom permissions during installation.

**Test Data:** Smapp Windows installer, Custom permissions

**Expected Result:** 

- Installation is successful.
- Permissions are set according to the custom settings.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-09

**Description:** Verify that an unofficial package (prerelease, custom build, etc.) can be installed on a Mac.

**Steps:**

1. Download the unofficial Smapp Mac package.

2. Attempt to install the package.

**Test Data:** Unofficial Smapp Mac package

**Expected Result:** 

- Installation process and result consistent with expectations for an unofficial package - there should be a warning about the missing signature/untrusted authors/potential threat.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-10

**Description:** Verify that an unofficial package (prerelease, custom build, etc.) can be installed on Windows.

**Steps:**

1. Download the unofficial Smapp Windows package.

2. Attempt to install the package.

**Test Data:** Unofficial Smapp Windows package

**Expected Result:** 

- Installation process and result consistent with expectations for an unofficial package - there should be a warning about the missing signature/untrusted authors/potential threat.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-11

**Description:** Verify that an unofficial package (prerelease, custom build, etc.) can be installed on Ubuntu.

**Steps:**

1. Download the unofficial Smapp Ubuntu package.

2. Attempt to install the package.

**Test Data:** Unofficial Smapp Ubuntu package

**Expected Result:** 

- Installation process and result consistent with expectations for an unofficial package.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-12

**Description:** Verify that Smapp can be installed and run on Windows without Visual C++ Redistributable.

**Steps:**

1. Uninstall or ensure Visual C++ Redistributable is not installed.

2. Install and run Smapp.

**Test Data:** Smapp Windows installer

**Expected Result:** 

- Appropriate error messages and node doesn't connect to the network.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-13

**Description:** Verify that Smapp can be installed and run on Windows without OpenCl support.

**Steps:**

1. Uninstall or disable OpenCl.

2. Install and run Smapp.

**Test Data:** Smapp Windows installer

**Expected Result:** 

- Appropriate error messages and node doesn't connect to the network, no way to get the GPU POS provider.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-14

**Description:** Verify that Smapp can be installed and run on Ubuntu without OpenCl support.

**Steps:**

1. Uninstall or disable OpenCl.

2. Install and run Smapp.

**Test Data:** Smapp Ubuntu package

**Expected Result:** 

- Appropriate behavior or error messages when OpenCl support is missing and node doesn't connect to the network, no way to get the GPU POS provider.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-15

**Description:** Verify that Smapp can be run via CLI with flags on macOS.

**Steps:**

1. Open Terminal.

2. Run Smapp with various CLI flags.

**Test Data:** CLI flags

**Expected Result:** 

- Smapp behaves as expected when run with various CLI flags.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-16

**Description:** Verify that Smapp can be run via CLI with flags on Windows.

**Steps:**

1. Open Command Prompt.

2. Run Smapp with various CLI flags.

**Test Data:** CLI flags

**Expected Result:** 

- Smapp behaves as expected when run with various CLI flags.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-17

**Description:** Verify that Smapp can be run via CLI with flags on Ubuntu.

**Steps:**

1. Open Terminal.

2. Run Smapp with various CLI flags.

**Test Data:** CLI flags

**Expected Result:** 

- Smapp behaves as expected when run with various CLI flags.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-18

**Description:** Verify rollback functionality if installation fails on Windows.

**Steps:**

1. Intentionally corrupt the installation process on Windows.

2. Observe rollback functionality.

**Test Data:** Corrupted Smapp Windows installer

**Expected Result:** 

- Installation should rollback to the previous state.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-19

**Description:** Verify rollback functionality if installation fails on Mac.

**Steps:**

1. Intentionally corrupt the installation process on Mac.

2. Observe rollback functionality.

**Test Data:** Corrupted Smapp Mac installer

**Expected Result:** 

- Installation should rollback to the previous state.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-20

**Description:** Verify rollback functionality if installation fails on Linux.

**Steps:**

1. Intentionally corrupt the installation process on Linux.

2. Observe rollback functionality.

**Test Data:** Corrupted Smapp Linux installer

**Expected Result:** 

- Installation should rollback to the previous state.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-21

**Description:** Verify Smapp behavior when disk space is insufficient for installation.

**Steps:**

1. Fill the disk to near capacity.

2. Attempt to install Smapp.

**Test Data:** Limited disk space

**Expected Result:** 

- Appropriate error message and halting of installation.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-22

**Description:** Installation over an older version of Smapp without uninstalling the old version on Windows.

**Steps:**

1. Install an older version of Smapp.

2. Install the new version without uninstalling the older version.

**Test Data:** Old and new versions of Smapp Windows installer

**Expected Result:** 

- New version should successfully install and replace the old version, retaining settings where applicable.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---
 #### Test Case ID: Install-23

**Description:** Installation over an older version of Smapp without uninstalling the old version on Mac.

**Steps:**

1. Install an older version of Smapp.
2. Install the new version without uninstalling the older version.

**Test Data:** Old and new versions of Smapp Mac installer

**Expected Result:** 

- New version should successfully install and replace the old version, retaining settings where applicable.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-24

**Description:** Installation over an older version of Smapp without uninstalling the old version on Linux.

**Steps:**

1. Install an older version of Smapp.
2. Install the new version without uninstalling the older version.

**Test Data:** Old and new versions of Smapp Linux installer

**Expected Result:** 

- New version should successfully install and replace the old version, retaining settings where applicable.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-25

**Description:** Verify the installer's digital signature on Windows.

**Steps:**

1. Download the Smapp installer for Windows.
2. Verify the digital signature.

**Test Data:** Smapp Windows installer

**Expected Result:** 

- The installer should have a valid digital signature.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-26

**Description:** Verify the installer's digital signature on Mac.

**Steps:**

1. Download the Smapp installer for Mac.
2. Verify the digital signature.

**Test Data:** Smapp Mac installer

**Expected Result:** 

- The installer should have a valid digital signature.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-27

**Description:** Verify that Smapp auto-updates to a new version.

**Steps:**

1. Install an older version of Smapp (signed package).
2. Check for updates.

**Test Data:** Older version of Smapp

**Expected Result:** 

- Smapp should auto-update to the latest version.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-28

**Description:** Verify Smapp's firewall rules on Windows.

**Steps:**

1. Install Smapp on Windows.
2. Check the firewall settings related to Smapp.

**Test Data:** Smapp Windows installer

**Expected Result:** 

- Firewall rules should be appropriately set for Smapp to function correctly.
- There might be a warning about the incoming connections, but no functionality should be blocked by Defender/Firewall

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-29

**Description:** Verify that Smapp doesn't affect system boot time.

**Steps:**

1. Measure system boot time without Smapp installed.
2. Install Smapp.
3. Measure system boot time with Smapp installed.

**Test Data:** System boot times

**Expected Result:** 

- System boot time should not be significantly impacted by the installation of Smapp.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-30

**Description:** Validate Smapp’s data folder structure post-installation.

**Steps:**

1. Install Smapp.
2. Navigate to Smapp’s data directory.

**Test Data:** Smapp installer

**Expected Result:** 

- Data folder structure should be as expected and contain all necessary files (to be updated with more details)

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-31

**Description:** Verify behavior when trying to install Smapp without admin rights.

**Steps:**

1. Log in to the system as a non-admin user.
2. Try to install Smapp.

**Test Data:** Smapp installer

**Expected Result:** 

- Smapp should not require admin rights to be installed

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

#### Test Case ID: Install-32

**Description:** Installing Smapp when an antivirus program is running.

**Steps:**

1. Ensure an antivirus program is active.
2. Install Smapp.

**Test Data:** Smapp installer

**Expected Result:** 

- Smapp should install without being flagged or blocked by the antivirus program.

**Actual Result:** [Save the actual result here after test execution]

**Status:** [Pass / Fail]

---

