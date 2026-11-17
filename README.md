# ci-images

Official `postgres` and `redis` images copied to GHCR, so CI jobs pull from
`ghcr.io/ederlonbarbosaprimebull/<image>:<tag>` instead of Docker Hub (no
anonymous pull limit). Refreshed weekly by `.github/workflows/mirror.yml`;
add a tag to the matrix to mirror it.

The packages must be public (Package settings > Change visibility > Public)
so other repos pull them without credentials.
