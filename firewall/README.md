# Firewall Policy Overview

This directory documents the firewall *policies* enforced by the
Gatepath infrastructure.

It intentionally does **not** contain full operational firewall rules.
Exact implementations, rule ordering, and infrastructure-specific
details are omitted.

The purpose of this documentation is to describe *what is enforced*,
not *how it is implemented*.

## High-level policies

- VPN traffic is restricted to explicitly allowed paths
- Tor-only paths have no clearnet egress
- Tor usage is explicit and opt-in
- No transparent proxying is used
- SSH access is restricted to trusted infrastructure only
- Ingress is limited to required services (e.g. WireGuard)

## Rationale

Publishing full firewall configurations would expose unnecessary
operational details without providing meaningful security benefits.

This repository focuses on design intent and trust boundaries.
