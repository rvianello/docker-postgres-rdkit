postgres-rdkit
==============

This repository provides a Dockerfile for extending the official PostgreSQL debian-based Docker image, with the installation of the RDKit cartridge.

Example command to build the image:

```bash
docker build -f Dockerfile  --build-arg postgres_image_version="12.17-bullseye" --build-arg postgres_version=12 --build-arg rdkit_git_ref=Release_2023_09_6  --tag rdkit-postgres-12-rdkit_2023_09_6:latest .
```

For everything related to how to run postgres, you should be able to just refer to the documentation for the [upstream image](https://hub.docker.com/_/postgres).

For everything related to how to use the RDKit cartridge, you can refer to the related [documentation](https://www.rdkit.org/docs/Cartridge.html).

