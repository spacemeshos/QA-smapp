# Test Scenario

#### Unique ID: Install

**Description:** Smapp installation process from 0 to running app

**Priority:** 1

**Prerequisites:** Internet connection, minimal system requirements met, Visual C++ Redistributable, OpenCl support

**Test Cases:**

[01](#test-case-id-install-01) - Getting the right package

[02]() - Checking the package security - Virustotal scan and checksum verification (currently for go-spacemesh only)

[03]() - Default installation process on Mac 

[04]() - Default installation process on Windows

[05]() - Default installation process on Linux (AppImage)

[06]() - Default installation process on Linux (.deb )

[07]() - Custom directory on Windows for installation

[08]() - Custom permissions on Windows (for other users)

[09]() - Getting the unofficial package (prerelease, custom build etc.) and trying to install it on Mac

[10]() - Getting the unofficial package (prerelease, custom build etc.) and trying to install it on Windows

[11]() - Getting the unofficial package (prerelease, custom build etc.) and trying to install it on Ubuntu

[12]() - Installing and running Smapp on Windows without Visual C++ Redistributable

[13]() - Installing and running Smapp on Windows without OpenCl support

[14]() - Installing and running Smapp on Ubuntu without OpenCl support

[15]() - Running Smapp via CLI with flags - macOS

[16]() - Running Smapp via CLI with flags - Windows

[17]() - Running Smapp via CLI with flags - Ubuntu




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