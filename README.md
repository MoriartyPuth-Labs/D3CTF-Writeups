# D^3CTF 2026 - Writeups

A comprehensive walkthrough writeup repository for key challenges from **D^3CTF 2026**, covering Web, Pwn, Misc, Cryptography, and Reverse Engineering.

---

## Challenge Index

| Category | Challenge Name | Difficulty | Core Concept / Vulnerability | Walkthrough Link |
| :--- | :--- | :---: | :--- | :--- |
| 🌐 **Web** | **Scope Drift** | Medium | Double URL-decoding path normalization leading to Service Worker scope hijacking | [View Walkthrough](web/scope-drift.md) |
| 🌐 **Web** | **Ghost Zero** | Hard | SQLite `sqlite_dbpage` recovery of deleted PCAP & ticket scope bypass | [View Walkthrough](web/ghost-zero.md) |
| ⚔️ **Pwn** | **d3kbus** | Hard | Kernel zero-copy CRC32C linear system solving page cache overwrite (DirtyFrag) | [View Walkthrough](pwn/d3kbus.md) |
| ⚔️ **Pwn** | **d3kheap2pro** | Hard | Kernel slab double-free with CPU Sheaf cache draining & `INIT_ON_ALLOC` cred zeroing | [View Walkthrough](pwn/d3kheap2pro.md) |
| 🧩 **Misc** | **proxyport** | Easy | FRP reverse proxy TCP half-closed state machine FIN packet handling discrepancy | [View Walkthrough](misc/proxyport.md) |
| 🔐 **Crypto** | **D3HFERP** | Hard | Overdetermined Multivariate Quadratic (MQ) system solved via Extended Linearization (XL) over $\mathbb{F}_3$ | [View Walkthrough](crypto/d3hferp.md) |
| 🔄 **Reverse** | **PacMan** | Hard | iOS Mach-O binary with distributed Mach-messaging bytecode VM & RC4 decryption | [View Walkthrough](reverse/pacman.md) |
| 🔄 **Reverse** | **d3llvm** | Hard | Android OLLVM-obfuscated library, 16-bit non-linear mixing network & AES-ECB decryption | [View Walkthrough](reverse/d3llvm.md) |

---

## Summary of Captured Flags

| Challenge | Flag |
| :--- | :--- |
| **Scope Drift** | `d3ctf{d0uble_url_dec0de_sw_sc0pe_dr1ft_pwned}` |
| **Ghost Zero** | `d3ctf{sql1_dbpage_pcap_rec0very_and_t1cket_expl01t}` |
| **d3kbus** | `d3ctf{d3kbus_dirtyfrag_pagecache_crc32c_pwn}` |
| **d3kheap2pro** | `d3ctf{cpu_sheaf_cross_cache_init_on_alloc_cred_zeroing}` |
| **proxyport** | `d3ctf{frp_tcp_fin_state_machine_detection_success}` |
| **D3HFERP** | `flag{S1mpl3_Att4ck_br34ks_HFERP_2026}` |
| **PacMan** | `d3ctf{mach_actor_vm_pacman_rc4_decrypted}` |
| **d3llvm** | `d3ctf{Hey5h4d0ww4lk3R-1d2efadd-aaef-zenu-s100}` |

---

## 🛠️ Repository Structure

```
.
├── README.md
├── web/
│   ├── scope-drift.md
│   └── ghost-zero.md
├── pwn/
│   ├── d3kbus.md
│   └── d3kheap2pro.md
├── misc/
│   └── proxyport.md
├── crypto/
│   └── d3hferp.md
└── reverse/
    ├── pacman.md
    └── d3llvm.md
```

---

## 📄 License
This repository is published under the [MIT License](LICENSE).
