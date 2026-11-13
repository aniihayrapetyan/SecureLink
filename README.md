\# SecureLink

\### Secure Inline Communication Channel Using Diffie–Hellman Key Exchange



SecureLink is a Linux-based C project that implements a prototype of a secure inline communication channel between two hosts through two intermediate network devices.



The system establishes a shared cryptographic session key using the Diffie–Hellman key exchange before protected TCP communication begins.



\## Project Architecture



```text

PC1

&#x20;|

&#x20;v

Device1

&#x20;|

&#x20;|  Secure session establishment

&#x20;|  Diffie–Hellman key exchange

&#x20;|  TCP payload encryption

&#x20;|

&#x20;v

Device2

&#x20;|

&#x20;v

PC2

```



\## Main Objectives



\- Establish a secure communication session between Device1 and Device2.

\- Implement Diffie–Hellman key exchange to derive a shared session key.

\- Process selected IPv4/TCP traffic.

\- Encrypt and decrypt TCP payload data while preserving packet headers.

\- Ensure that protected data is transmitted only after session establishment.



\## Technologies Used



\- \*\*Programming Language:\*\* C

\- \*\*Operating System:\*\* Linux

\- \*\*Networking:\*\* TCP/IP, IPv4

\- \*\*Cryptography:\*\* Diffie–Hellman key exchange

\- \*\*Build System:\*\* GNU Make



\## Repository Structure



```text

SecureLink/

├── config/       # Configuration files

├── docs/         # Project documentation

├── include/      # Header files

├── scripts/      # Helper scripts

├── src/          # C source files

├── tests/        # Test files

├── LICENSE

├── Makefile

└── README.md

```



\## Installation



Clone the repository:



```bash

git clone https://github.com/anihayrapetyan/SecureLink.git

cd SecureLink

```



Build the project:



```bash

make

```



\## System Requirements



\- Linux environment

\- GCC compiler

\- GNU Make

\- Required cryptographic and networking dependencies specified by the project



\## Testing



The `tests/` directory contains the project's test resources.



Run the tests using the commands defined in the project Makefile.



\## Security Considerations



SecureLink is an educational and experimental prototype. It is intended for demonstrating secure network communication concepts and should not be considered production-ready without further security analysis, testing, and hardening.



\## Project Goals



This project explores practical network security concepts, including key exchange, session establishment, packet processing, and payload encryption.



\---



\*\*Author:\*\* Ani Hayrapetyan  

\*\*Project:\*\* SecureLink  

\*\*Language:\*\* C

