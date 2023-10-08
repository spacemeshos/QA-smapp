# Contributing to QA-smapp

:wave: Hi there! Thank you for your interest in contributing to the Spacemesh QA-smapp repository. This document outlines how you can contribute to improving and evolving this part of the Spacemesh ecosystem.

## Table of Contents

1. [Pull Requests](#pull-requests)
2. [Coding Guidelines](#coding-guidelines)
3. [Documentation](#documentation)
4. [Testing](#testing)
5. [Issue Reporting](#issue-reporting)


---

## Pull Requests

1. Before you submit a PR, please ensure you've followed the getting started guide and adhere to our [Coding Guidelines](#coding-guidelines).
2. Make sure to add a detailed explanation of your work, so our maintainers understand the purpose behind the PR.
3. After you've created your PR, our team will review your contribution and provide feedback.

---

## Coding Guidelines

### Electron

- Follow Electron's best practices as outlined in their [documentation](https://www.electronjs.org/docs/latest/tutorial/automated-testing).

### Test Automation - JavaScript

- Use consistent indentation and follow the style guidelines for JavaScript.
- Write modular, reusable code. Aim to make your functions small and focused.
- Comment your code where necessary to clarify complex logic or decisions made.
- Please include necessary assertions to verify that a test does what it claims to do.

### Test Automation - Python

- Follow PEP 8, the Python programming style guide, available at [PEP 8 -- Style Guide for Python Code](https://www.python.org/dev/peps/pep-0008/).
- Comment your code effectively, especially if you're writing complex algorithms.
- Always provide meaningful assert messages to make it easy to identify the reason for test failures.

---

## Documentation

If you are adding new test cases or making significant changes to existing ones, please document them using the specified test scenario and test case template.

---

## Testing

### Automated Testing

- **Write Comprehensive Tests**: Ensure that tests cover as many scenarios as possible, from standard cases to edge cases.
  
- **Consistency**: Maintain a consistent naming convention and organizational structure for test files and test cases. This makes it easier to locate and manage tests.
  
- **Review Test Failures**: Any failing test should be reviewed and fixed before submitting a Pull Request. If a test fails due to reasons beyond your code, document it.

- **Test Isolation**: Each test should be independent and be able to run in any order. Avoid writing tests that rely on other tests.

- **Environment**: Ensure that tests can run in any environment, be it a local developer machine, CI server, or any other system.

### Manual Testing

- **Regression Testing**: After implementing a feature or fix, run relevant tests to ensure that the existing functionality is not broken.
  
- **Cross-platform Testing**: Manually test the application on different operating systems and browsers to ensure cross-platform compatibility.

- **User Experience**: Occasionally perform manual checks to ensure that the user experience is smooth and intuitive. Automated tests might not capture issues related to UI/UX.

### Reporting

- **Automated Test Reports**: Utilize tools that produce test reports to ensure you can quickly grasp the state of the application's health.
  
- **Issue Tracker**: Any defects or issues found during testing should be promptly reported in the GitHub Issues section following the reporting guidelines.


---

## Issue Reporting

- Use GitHub Issues to report bugs, request features, and discuss improvements.
- Before creating a new issue, please check to make sure a similar issue doesn't already exist.

---

Thank you for helping make QA-smapp a better tool for everyone in the Spacemesh community!

---
