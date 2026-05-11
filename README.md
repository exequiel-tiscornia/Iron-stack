**Iron Stack**  
*Post-Quantum Anonymous P2P Transport Protocol*

**Iron Stack** is a UDP transport stack built from the ground up for a world where quantum computers exist. It combines post-quantum cryptography, onion routing, anonymous peer-to-peer communication, and traffic obfuscation into a single, coherent system — not an assembly of tools, but a protocol designed as an integrated foundation.

It is not a VPN. It is not a proxy. It is a **low-level transport infrastructure layer** upon which secure applications, anonymous communication tools, distributed systems, and privacy-critical services can be built.

### The Problem

Today’s encrypted internet relies on cryptographic primitives that will be broken by sufficiently powerful quantum computers. RSA, ECDH, and ECDSA — the backbone of TLS, Signal, WireGuard, and most secure systems — are theoretically vulnerable to Shor’s algorithm. The question is not if, but when.

Beyond the quantum threat, current secure communication tools suffer from structural weaknesses: centralized infrastructure, metadata leakage, traffic analysis, and persistent identities across sessions.

Iron Stack was built to address all of these challenges simultaneously.

### Core Architecture

- **Post-Quantum Cryptography**: Kyber-1024 (KEM) and Falcon (signatures), with modular design for future upgrades.
- **Transport Layer**: UDP with BBR congestion control, Weighted Fair Queuing (WFQ), stream multiplexing, reliable delivery, and 0-RTT session tickets.
- **Ghost Network**: Multi-hop onion routing (3-5 hops by default) with pre-built circuit pools and fixed-size cells to resist traffic analysis.
- **Anti-Analysis & Obfuscation**: Cover traffic, random payload segmentation, and Protocol Mimic (can masquerade as TLS 1.3, QUIC, or HTTP/1.1).
- **Ghost Rooms**: Encrypted multi-party rooms with messaging, file transfer, and distributed Virtual File System (VFS).
- **Ephemeral Mode**: Zero disk footprint execution with strong kernel hardening (landlock, seccomp, mlockall, etc.).
- **Gossip Cluster**: Distributed peer discovery with anti-Sybil, anti-cloning, and Shamir Secret Sharing for identity recovery.

### Current Status

- Functional network with multiple nodes in WAN environments.
- Stable circuit construction and pool management.
- Anonymous chat, file transfer, and distributed VFS operational.
- Ephemeral mode with advanced security measures.


The system is in an advanced stage of development, approaching a closed beta.

### Opportunity

Iron Stack represents a new foundation for secure communications in the post-quantum era. It can serve as the base for:

- Anonymous and censorship-resistant communication systems
- Privacy-focused distributed applications
- Secure P2P tools (chat, file sharing, collaboration)
- Resilient mesh networks

**We are looking for**  
Technical investors, strategic partners, and organizations interested in post-quantum and privacy infrastructure to collaborate on the next phase: final stabilization, external security audit, and initial production deployments.

contact: ironstackpq@proton.me
