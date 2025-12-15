# Upstream Tracking

This repository is a Tinyland fork of Sunshine (LizardByte), maintained for custom builds targeting Darwin (macOS) and Rocky Linux 10.

## Upstream Source

- **Repository:** LizardByte/Sunshine
- **URL:** https://github.com/LizardByte/Sunshine
- **License:** GPL-3.0
- **Documentation:** https://docs.lizardbyte.dev/projects/sunshine

## Tinyland Modifications

- Darwin (macOS) PKG builds with Developer ID signing and notarization
- Rocky Linux 10 RPM packages
- REST API enhancements for automated pairing

## Sync Status

- **Last Synced:** 2025-12-15
- **Upstream Branch:** master
- **Sync Method:** Renovate + manual merge

## API Endpoints

Sunshine provides REST API at `https://<host>:47990/api/`:
- `POST /api/pin` - Submit pairing PIN
- `GET /api/clients/list` - List paired clients
- `POST /api/clients/unpair` - Unpair a client

## Security Notes

- GHSA-3hrw-xv8h-9499: Fixed in 0.24.0+ (pairing protocol vulnerability)
- GHSA-jqph-8cp5-g874: Fixed (state management during pairing)
