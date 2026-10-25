# Amaterasu protocol source (publication candidate)

This source repository holds GameStream wire/crypto code plus the input and
network policy and identity crates. It does not start a listener or grant
network or input access. Its source originated in committed Amaterasu
`a6b0db9e36a1a59328ab4b4785b27b210f8182b7`; the extracted protocol
implementation is unchanged.

`Cargo.toml` pins the proposed `nonary-streams/amaterasu-sdk` source URL and
an exact SDK commit. `Cargo.lock` records the validated resolution. After that
repository has been published at the pinned commit, run
`cargo test --workspace --locked`. The two UDP loopback binding tests need a
network-capable isolated test environment; the remaining tests can run with
`--offline` and those two names skipped. A local mirror was used to validate
the proposed Git identity before any remote existed. No protocol artifact or
host runtime was published or activated by this preparation.

Amaterasu owns this repository. External developers consume its versioned
crates from independent extension repositories; source visibility does not
grant access to change Amaterasu or to register host services. The public
source license and release tags remain to be decided.
