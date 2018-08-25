# Docker release files

Dockerfile, dockerignore, docker.env, and a makefile for releasing images, based on Distillery 2.0 docs.

Assumptions:

- Distillery is installed and configured
- npm is used over yarn for local development

```bash
make image
```

To use a custom node version:

```
make image NODE_VERSION 8.9.4
```

run the latest release with:

```bash
make run
```

run migrations with `make task`, and the name of the task defined in your distillery config.

```bash
make task create
```
