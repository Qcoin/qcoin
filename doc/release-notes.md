1.0.0.2 beta changes
=============
- openssl-1.0.1k or older versions patched for CVE-2014-8275 broke compatibility with Bitcoin and Qcoin.
 This update patches Qcoin to maintain compatibility with CVE-2014-8275 patched openssl.
- If you are running v1.0.0.2 as distributed by qcoin.co you do not need to upgrade.
 The binaries distributed on qcoin.co contain their own copy of openssl so they are unaffected by this issue.

1.0.0.1 beta
=============
- Upgrade OpenSSL to 1.0.1i (see https://www.openssl.org/news/secadv_20140806.txt - just to be sure, no critical issues for Bitcoin Core)
- Enforce v2 blocks at height 710000 on mainnet, 400000 on testnet
- Add `-maxorphantx=<n>` and `-maxorphanblocks=<n>` options for control over the maximum orphan transactions and blocks
- Stricter memory limits on CNode
- Upgrade OpenSSL to 1.0.1i (see https://www.openssl.org/news/secadv_20140806.txt - just to be sure, no critical issues