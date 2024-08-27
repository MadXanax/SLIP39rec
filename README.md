# SLIP39rec(overy) : Shamir Seed Recovery Tool

A Python tool to recover a BIP39 24-word seed phrase from Shamir Secret Shares (SLIP39), following a secure and user-friendly process. This tool mimics Trezor's implementation to provide a reliable method for seed phrase reconstruction using multiple mnemonic shares.

Features
--------
- **Mnemonic Share Validation**: Ensures that each SLIP39 mnemonic share provided is valid and correctly formatted.
- **Secure Data Handling**: Implements secure deletion of sensitive data from memory to reduce exposure risk.
- **Dynamic Share Input**: Dynamically gathers the required number of mnemonic shares based on the SLIP39 configuration.
- **Seed Phrase Reconstruction**: Combines mnemonic shares to recover the original seed phrase, with optional passphrase support.
- **User-Friendly Interface**: Command-line interface for easy interaction, guiding users through each step of the recovery process.

Installation
------------

```bash
git clone https://github.com/MadXanax/SLIP39rec.git
cd SLIP39rec
pip install -r requirements.txt
python Recombine_ShamirShares_into_seedphrase.py


Usage
-----
Run the script:

python shamir_seed_recovery.py
Follow the prompts to input your mnemonic shares. The tool will validate each share and dynamically calculate the required number of shares needed for recovery.

Optionally, input a passphrase if one was used during the creation of the shares.

Recover the seed phrase: The tool will reconstruct the original seed phrase and display it on the screen.
