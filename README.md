## Overview

This repository contains the Quality Assurance (QA) assets for the Smapp application.

_Knowing that there will be huge changes in the GUI, this repo will not be perfectly maintained and docs meticulously prepared. It's more about gathering the core functions testing aspects than official documentation._

Smapp is an Electron-based application designed for managing wallets and facilitating the process of mining Smesh coins.

This repo includes test cases, test scripts, and documentation for testing the application across Windows, macOS, and Linux platforms.

## Table of Contents

- [Getting Started](#getting-started)
- [Test Scenarios](#test-scenarios)
  - [Smapper](#smapper)
  - [Smesher](#smesher)
- [Template](#template)
- [Contribution Guidelines](#contribution-guidelines)
- [License](#license)

## Getting Started

To get started with testing Smapp, clone this repository and follow the instructions in each test case.

```bash
git clone https://github.com/spacemeshos/QA-smapp.git
```

## Test Scenarios

### Smapper

* [Installation](cases/Smapper/Installation.md)
* [Login](cases/Smapper/Login.md)
* [Log Out](cases/Smapper/LogOut.md)
* [Autostart](cases/Smapper/Autostart.md)
* [Wallet Only Creation](cases/Smapper/WalletOnly-creation.md)
* [Password Setup](cases/Smapper/Password-setup.md)
* [Password Change](cases/Smapper/Password-change.md)
* [Additional Account](cases/Smapper/Additional-Account.md)
* [File Backup](cases/Smapper/File-backup.md)
* [File Restore](cases/Smapper/File-restore.md)
* [Mnemonics Backup](cases/Smapper/Mnemonics-backup.md)
* [Mnemonics Restore](cases/Smapper/Mnemonics-restore.md)
* [Spawn](cases/Smapper/Spawn.md)
* [Send](cases/Smapper/Send.md)
* [Export Transactions History](cases/Smapper/ExportTxLog.md)
* [Filter Transactions History](cases/Smapper/FilterTxLog.md)
* [Offline Modal](cases/Smapper/Offline-modal.md)

To be continued, work in progress...

### Smesher

* [POS General](cases/Smesher/POS_general.md)
* [POS Benchmark](cases/Smesher/POSbenchmark.md)
* [POS Coinbase](cases/Smesher/POScoinbase.md)
* [POS Delete](cases/Smesher/POSdelete.md)
* [POS Directory](cases/Smesher/POSdiectory.md)
* [POS Processor](cases/Smesher/POSprocessor.md)
* [POS Size](cases/Smesher/POSsize.md)
* [POS Summary](cases/Smesher/POSsummary.md)
* [POS Wallet + Node creation](cases/Smesher/WalletNode.md)

To be continued, work in progress...

## Template

For creating new test scenarios and cases, please use the [Scenario &amp; Test Case Template](cases/scenario-case-template.md).

## Contribution Guidelines

Please read the [Contribution Guidelines](CONTRIBUTING.md) before making any contributions.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
