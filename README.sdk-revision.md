# SDK dependency alignment

This source snapshot pins the reviewed hook-capable foundation commit
`fe3004d5889df3eb0ce6f68c74fbef0f33c76e94`. All protocol source code
and fixtures remain unchanged from the earlier extracted revision. Input
consumers should use this exact protocol revision alongside the same foundation
revision to avoid duplicate ABI/contract crate identities. No hook runtime is
implemented in this protocol repository, and no live service is activated.
