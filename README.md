# Declarative Enterprise ERP Infrastructure Configuration

This repository documents the custom system architecture deployment and orchestration configurations used to implement an enterprise-grade ERPNext environment on a hardened Linux stack.

## Infrastructure Highlights
- **Target OS Engine:** NixOS (Immutable, declarative host baseline to eliminate system drift).
- **Orchestration Matrix:** Docker Compose multi-container mesh isolating backend runtime workers, Redis state caches, asynchronous background queues, and a stateful MariaDB transactional database.
- **Network Architecture:** Automated ingress routing multiplexed with a Tailscale secure peer-to-peer overlay mesh network.

## Open Source Compliance Notice
This repository functions exclusively as an infrastructure configuration deployment portfolio. The core application services utilize upstream open-source packages maintained by the Frappe community under the GNU General Public License. No source application logic has been rewritten or re-invented here.
