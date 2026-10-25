# Amaterasu protocol source

This source repository holds GameStream wire/crypto code plus the input and
network policy and identity crates. It does not start a listener or grant
network or input access. Its source originated in committed Amaterasu
`a6b0db9e36a1a59328ab4b4785b27b210f8182b7`; the extracted protocol
implementation is unchanged.

`Cargo.toml` pins the public `nonary-streams/amaterasu-sdk` source URL and
an exact SDK commit. `Cargo.lock` records the validated resolution. To build the pinned dependency, run
`cargo test --workspace --locked`. The two UDP loopback binding tests need a
network-capable isolated test environment; the remaining tests can run with
`--offline` and those two names skipped. The public Git source is available; no binary protocol artifact or host
runtime has been installed or activated by publishing it.

Amaterasu owns this repository. External developers consume its versioned
crates from independent extension repositories; source visibility does not
grant access to change Amaterasu or to register host services. Project-authored
source is MIT licensed; release tags remain to be decided.
