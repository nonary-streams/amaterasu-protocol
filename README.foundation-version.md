# Foundation revision alignment

This input integration source snapshot pins ABI and contracts to foundation
`28da5667f73e26d812b0e485f50f0a5c77c5e4f0`, which also contains shared
storage. The earlier v0.1 protocol tag remains intact. Input must use this
same foundation revision for its SDK/media/storage dependencies so Cargo does
not instantiate duplicate ABI or contract crates from different Git revisions.
The `file://` source location is local-only and will require a stable approved
repository URL plus a regenerated lockfile before distribution.
