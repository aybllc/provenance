# aybllc/provenance

Single house for all custody records, checksums, and provenance across all research outputs.

**What lives here:** file manifests, SHA256 checksums, read-pass records, chain-of-custody notes  
**What does NOT live here:** manuscripts, gate logic, data, code  
**Author:** Eric D. Martin (ORCID 0009-0006-5944-1742)

## Structure

```
paper3-mnras/       — Paper 3 (Pantheon+ H0/Omega sensitivity)
paper2-uha/         — Paper 2 (Triple hierarchy)
paper1-mnras/       — Paper 1 (Hubble tension as measurement artifact)
```

Each directory contains:
- `photo_manifest.sha256` — SHA256 checksums of physical annotation photos
- `*_manifest.md` — human-readable custody record with page map and location of files

## Verify a custody record

```bash
cd paper3-mnras
sha256sum -c photo_manifest.sha256
```
