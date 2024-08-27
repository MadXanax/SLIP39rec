# SLIP39rec(overy) : Shamir Seed Recovery Tool

A Python tool to recover a BIP39 24-word seed phrase from Shamir Secret Shares (SLIP39), following a secure and user-friendly process. This tool mimics Trezor's implementation to provide a reliable method for seed phrase reconstruction using multiple mnemonic shares.

## Features

- **Mnemonic Share Validation**: Ensures that each SLIP39 mnemonic share provided is valid and correctly formatted.
- **Secure Data Handling**: Implements secure deletion of sensitive data from memory to reduce exposure risk.
- **Dynamic Share Input**: Dynamically gathers the required number of mnemonic shares based on the SLIP39 configuration.
- **Seed Phrase Reconstruction**: Combines mnemonic shares to recover the original seed phrase, with optional passphrase support.
- **User-Friendly Interface**: Command-line interface for easy interaction, guiding users through each step of the recovery process.

## Installation

```bash
git clone https://github.com/yourusername/shamir-seed-recovery.git
cd shamir-seed-recovery
pip install -r requirements.txt
