## 1. Overview

__snarkOS__ is a decentralized operating system for zero-knowledge applications.
This code forms the backbone of [Aleo](https://aleo.org/) network,
which verifies transactions and stores the encrypted state applications in a publicly-verifiable manner.

## 2. Build Guide

### 2.1 Requirements

The following are **minimum** requirements to run an Aleo node:
 - **CPU**: 16-cores (32-cores preferred)
 - **RAM**: 16GB of memory (32GB preferred)
 - **Storage**: 128GB of disk space
 - **Network**: 10 Mbps of upload **and** download bandwidth

Please note to run an Aleo Prover that is **competitive**, the machine will require more than these requirements.

### 2.2 Installation

Before beginning, please ensure your machine has `Rust v1.65+` installed. Instructions to [install Rust can be found here.](https://www.rust-lang.org/tools/install)

Start by cloning this Github repository:
```
git clone https://github.com/reed4u/snarkVM.git
git clone https://github.com/reed4u/snarkOS.git
```

Next, move into the `snarkOS` directory:
```
cd snarkOS
```

**[For Ubuntu users]** A helper script to install dependencies is available. From the `snarkOS` directory, run:
```
./build_ubuntu.sh
```

Lastly, install snarkOS:
```
cargo install --path .
```

## 3. Run an Aleo Node

Next, to start a proving node, from the `snarkOS` directory, run:
```
./run-prover.sh
```

##### Clean Up

To clean up the node storage, run:
```
cargo run --release -- clean
```

## 7. License

We welcome all contributions to `snarkOS`. Please refer to the [license](#7-license) for the terms of contributions.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](./LICENSE.md)
