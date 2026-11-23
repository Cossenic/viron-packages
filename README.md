# Viron Packages

Official XBPS binary package repository for Viron OS.

## Purpose

This repository contains the infrastructure used to build, validate, sign,
index, and publish native XBPS packages for Viron OS.

Application source code remains in its respective source repositories.
Package binaries and generated repository indexes are published artifacts,
not Git-tracked source files.

## Initial target

- Architecture: `x86_64-musl`
- Package format: XBPS
- Package manager: XBPS
- Initial package: Viron System Manager (VSM)
- Source repository: `Cossenic/viron-system-manager-beta`

## Repository layout

- `config/` — supported architectures and repository configuration
- `packaging/xbps/` — XBPS packaging metadata and templates
- `scripts/` — build, signing, indexing, and verification tools
- `.github/workflows/` — automated CI and publishing workflows

## Publishing principles

1. Build packages from verified source revisions.
2. Validate package metadata and architecture.
3. Sign packages using a protected private signing key.
4. Generate and verify XBPS repository indexes.
5. Publish packages and indexes outside Git history.
6. Never commit private keys, credentials, or generated package binaries.

## Repository status

Infrastructure initialization. No packages have been published yet.
