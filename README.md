# Amaterasu protocol source proof

Extracted from committed Amaterasu `a6b0db9e36a1a59328ab4b4785b27b210f8182b7`. This local-only
workspace retains GameStream wire/crypto code and the existing input/network
policy and identity crates used by multiple native modules. It pins the shared
ABI and control contracts to foundation commit `51ef23b1923335e0bb0c6af9eef685c6f4807520`.

No remote is configured. `file://` Git dependencies prove exact local source
pinning only; they require an approved stable URL and a regenerated lockfile
before cross-machine release builds. Protocol fixtures remain in their original
crate directories. No runtime service, input grant, network listener, or signed
release policy is created or changed by this extraction.
