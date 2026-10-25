# Historical SDK revision note

The v0.3 extraction pinned foundation
`fe3004d5889df3eb0ce6f68c74fbef0f33c76e94` while leaving protocol source
unchanged. This is provenance for that earlier source tag, not the current
build pin. Use the exact SDK revision in `Cargo.toml` and its committed
`Cargo.lock` for this publication candidate. Every downstream module must pin
compatible SDK and protocol revisions to avoid duplicate ABI crate identities.
No live protocol service is activated by this source repository.
