# SLIP39rec(overy)

A Python tool to recover a BIP39 seed phrase from Shamir Secret Shares (SLIP39), following a secure and user-friendly process. This tool mimics Trezor's implementation to provide a reliable method for seed phrase reconstruction using multiple mnemonic shares.

Features
--------
- **Mnemonic Share Validation**: Ensures that each SLIP39 mnemonic share provided is valid and correctly formatted.
- **Secure Data Handling**: Implements secure deletion of sensitive data from memory to reduce exposure risk.
- **Dynamic Share Input**: Dynamically gathers the required number of mnemonic shares based on the SLIP39 configuration.
- **Seed Phrase Reconstruction**: Combines mnemonic shares to recover the original seed phrase, with optional passphrase support.
- **User-Friendly Interface**: Command-line interface for easy interaction, guiding users through each step of the recovery process.

Installation
------------

Clone the repository:

    git clone https://github.com/MadXanax/SLIP39rec.git

Navigate to the project directory:

    cd SLIP39rec

Install required dependencies:

    pip install -r requirements.txt



Usage
-----
Run the script:

    python Recombine_ShamirShares_into_seedphrase.py

Follow the prompts to input your mnemonic shares. The tool will validate each share and dynamically calculate the required number of shares needed for recovery.

Optionally, input a passphrase if one was used during the creation of the shares.

Recover the seed phrase: The tool will reconstruct the original seed phrase and display it on the screen.

Exemple
-
```
=================== START ===================

 Enter the first mnemonic share:
[Your First Mnemonic Share]

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Deduced Parameters:
 -> Member Threshold (Shares needed to reconstruct): 3
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

 Enter Share 2 (use spaces to separate words):
[Your Second Mnemonic Share]

 Enter Share 3 (use spaces to separate words):
[Your Third Mnemonic Share]

Enter the secret-passphrase (leave empty if none was used, which is default): [Your Passphrase]

Original Seed Phrase Reconstructed:
---------------------------------------------
[Your Reconstructed Seed Phrase]
---------------------------------------------

=================== END N ===================
```
Security Considerations
-----------------------
* Data Deletion: The tool uses secure deletion methods to clear sensitive data from memory after use.
* Environment: Run this tool in a secure, offline environment (such as an air-gapped computer) to minimize risks.

Contributing
------------
Contributions are welcome! Please fork this repository and open a pull request to contribute to the project. For feature requests or bug reports, open an issue.

License
-------
This project is licensed under the GPL-3.0 license - see the LICENSE file for details.
