ARG UV_VERSION=0.5.13
ARG DEBIAN_VERSION=bookworm


FROM ghcr.io/astral-sh/uv:$UV_VERSION AS uv
FROM mcr.microsoft.com/vscode/devcontainers/base:$DEBIAN_VERSION

# Install pre-commit
RUN apt-get update \
    && apt-get install pre-commit -y 

COPY --from=uv --chown=vscode: /uv /uvx /bin/