# Valkey

Valkey clusters managed by the
[Valkey Kubernetes Operator](https://github.com/valkey-io/valkey-operator),
wrapped as an OpenEverest provider.

Supports replication and sharded cluster topologies. Operator is early-stage, far from production.

## Source

- **Provider repo:** https://github.com/openeverest/provider-valkey
- **Chart:** `oci://ghcr.io/openeverest/charts/provider-valkey`

## Install (manual)

> The OpenEverest CLI install path (`everestctl extension install`) ships in
> Phase 2. Until then, use Helm directly:

```bash
helm install provider-valkey \
  oci://ghcr.io/openeverest/charts/provider-valkey \
  --version 0.1.3 \
  --namespace everest-system \
  --create-namespace
```

The Valkey operator ships as a bundled Helm subchart and is installed
automatically with the provider — no separate install step is required.
