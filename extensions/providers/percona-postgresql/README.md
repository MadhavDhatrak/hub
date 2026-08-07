# Percona Distribution for PostgreSQL

PostgreSQL clusters managed by the
[Percona Operator for PostgreSQL](https://github.com/percona/percona-postgresql-operator)
(v3.0.x),
wrapped as an OpenEverest **provider**.

Supports cluster topology with pgBouncer proxy and PostgreSQL versions 14 through 18.

## Source

- **Provider repo:** https://github.com/openeverest/provider-percona-postgresql
- **Chart:** `oci://ghcr.io/openeverest/charts/provider-percona-postgresql`

## Install (manual)

> The OpenEverest CLI install path (`everestctl extension install`) ships in
> Phase 2. Until then, use Helm directly:

```bash
helm install provider-percona-postgresql \
  oci://ghcr.io/openeverest/charts/provider-percona-postgresql \
  --version 0.1.0 \
  --namespace everest-system \
  --create-namespace
```
