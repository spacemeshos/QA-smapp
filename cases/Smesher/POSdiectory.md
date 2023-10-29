

1. **Test Case: Directory Picker Invocation**

   * Description: Verify if the directory picker dialog opens upon clicking the link.
   * Expected Result: The dialog for choosing a directory should open without errors.
2. **Test Case: Directory Picker Cancelation**

   * Description: Ensure the directory picker dialog can be canceled without any side effects.
   * Expected Result: Canceling the dialog should not select any directory, and previously selected directory (if any) remains unchanged.
3. **Test Case: Valid Directory Selection**

   * Description: Check if a valid directory selection enables the 'Next' button.
   * Expected Result: The 'Next' button becomes active when a valid, empty directory is chosen.
4. **Test Case: Invalid Directory Selection - Non-empty Directory**

   * Description: Confirm that selecting a non-empty directory shows a warning.
   * Expected Result: A warning is displayed, and the PoS process does not start.
5. **Test Case: Sufficient Free Disk Space Verification**

   * Description: Verify that the 'Next' button is enabled when the directory has more than the required free disk space.
   * Expected Result: The 'Next' button is active when there is sufficient free disk space.
6. **Test Case: Insufficient Free Disk Space Verification**

   * Description: Check if the 'Next' button is disabled when there's not enough free disk space.
   * Expected Result: The 'Next' button is disabled, and the user is possibly warned about insufficient space.
7. **Test Case: Display of Free Space**

   * Description: Verify that the free space in the chosen directory is accurately displayed.
   * Expected Result: The note shows the correct amount of free disk space.
8. **Test Case: Refresh of Free Space Info on Directory Change**

   * Description: Ensure that the free space information updates when a different directory is selected.
   * Expected Result: The displayed free disk space updates to reflect the new directory's free space.
9. **Test Case: Cancel Button Functionality**

   * Description: Verify that the 'Cancel' button cancels the PoS directory selection process.
   * Expected Result: Clicking 'Cancel' exits the directory selection process without proceeding to the next step.
10. **Test Case: File System Permissions**

    * Description: Verify that the application handles the selection of a directory with restricted permissions correctly.
    * Expected Result: The application should either not allow the selection of such a directory or should display an appropriate warning message.
11. **Test Case: Selection of Removable Media**

    * Description: Confirm that selecting a directory on removable media is handled properly.
    * Expected Result: The application should either prevent selection if it's not supported or should warn about potential issues with removable media.
12. **Test Case: Reacting to External Changes in Directory**

    * Description: Verify the application's behavior if the chosen directory is modified outside the app (e.g., files added/removed externally).
    * Expected Result: The application should detect changes and update the display/enable/disable 'Next' button accordingly.
13. **Test Case: Network Location Selection**

    * Description: Assess the behavior when a network location is selected as the PoS directory.
    * Expected Result: If supported, the application should handle it correctly; if not supported, it should provide a clear message.
14. **Test Case: Retry after Warning**

    * Description: Test the ability to reselect a directory after being warned that the previous selection was non-empty.
    * Expected Result: User should be able to choose a different directory without any issues following a warning.
15. **Test Case: Next Button State Persistence**

    * Description: Check if the state of the 'Next' button persists correctly when navigating back to the first step after advancing in the setup process.
    * Expected Result: The 'Next' button should retain its enabled/disabled state based on the previous interactions
16. **Test Case: Directory Selection Persistence**

    * Description: Verify that the selected directory is remembered if the user navigates to the next step and then returns back to the directory selection step.
    * Expected Result: The previously selected directory should still be selected upon returning to the directory selection step.
17. **Test Case: Directory Selection After Warning**

    * Description: Check if the user can select a new directory after receiving a warning for choosing a non-empty directory.
    * Expected Result: The user should be able to select a new directory, and the application should update accordingly.
18. **Test Case: Directory Path Length**

    * Description: Ensure the application can handle long directory paths beyond typical filesystem limits.
    * Expected Result: The application should either accept the long path or display a message stating path length limitations.
19. **Test Case: Directory with Hidden Files**

    * Description: Confirm that selecting a directory that contains hidden files or system files triggers the non-empty directory warning.
    * Expected Result: The application should recognize the directory as non-empty and warn the user.
20. **Test Case: Reactivity to Disk Space Changes (not implemented afaik, might be in smapp2)**

    * Description: Check if the application updates the free space note and 'Next' button status in real-time as disk space changes.
    * Expected Result: The note and the 'Next' button's status should reflect the current state of the disk space without needing to reopen or refresh the application.
21. **Test Case: Choosing a Directory with Symlinks**

    * Description: Test the application's behavior when selecting a directory that contains symlinks.
    * Expected Result: The application should correctly handle symlinks within the directory, either by following them or ignoring them, based on the intended design. (to be checked)
22. **Test Case: Directory Selection on Different File Systems**

    * Description: Verify that the application can handle directory selection across different filesystems (e.g., NTFS, FAT32, exFAT, ext4).
    * Expected Result: The application should either support all these filesystems or provide clear messaging about any limitations.
23. **Test Case: Impact of Disk Space Requirement on System Performance**

    * Description: Assess the impact on system performance when the minimum required disk space is nearly consumed.
    * Expected Result: The application should warn the user if the disk space usage might affect system performance or if it's too close to the limit.
24. **Test Case: Multiple Directory Selection Attempts**

    * Description: Ensure the application can handle multiple directory selection attempts without crashing or displaying incorrect information.
    * Expected Result: Users should be able to attempt directory selection multiple times with consistent and accurate feedback from the application.
25. **Test Case: Error Handling for File System Errors**

    * Description: Test how the application handles unexpected file system errors during directory selection (e.g., read/write permissions, disk errors).
    * Expected Result: The application should display an appropriate error message and not allow the user to proceed with an invalid selection.
26. **Test Case: Language and Encoding Support in Directory Paths**

    * Description: Verify that the application supports directory paths with non-English characters and various encodings.
    * Expected Result: The application should properly handle paths with a variety of characters and encodings without errors.
27. **Test Case: User Interface Responsiveness**

    * Description: Test the responsiveness of the user interface when interacting with the directory picker on systems with low resources.
    * Expected Result: The directory picker should remain responsive and should not cause the application to hang or crash.
28. **Test Case: Handling of External Drives Being Ejected**

    * Description: Check the application's behavior if the selected directory is on an external drive that gets ejected.
    * Expected Result: The application should handle this gracefully, either by prompting the user to re-select a directory or by displaying a clear warning message.
