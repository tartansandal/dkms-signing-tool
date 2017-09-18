# dkms-signing-tool

A helper script to assist with signing DKMS modules so that systems can run
with Secure Boot enabled.

The intention is to encourage good security practices by encasulating them in
a tool.

## Intended Features/Functions

* prepare a luks encrypted USB drive for storing keys
* create a key pair appropriate for module signing
* adding new key to the MOK key ring
* disabling previously added keys
* detect unsigned dkms modules and prompt for resigning
* search for and sign all dkms modules with the same key
