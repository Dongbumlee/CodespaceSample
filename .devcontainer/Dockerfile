ARG UV_VERSION=0.5.22
ARG Py_VERSION=3.12


FROM ghcr.io/astral-sh/uv:$UV_VERSION AS uv
FROM mcr.microsoft.com/vscode/devcontainers/python:${Py_VERSION}

# Install pre-commit
RUN apt-get update \
    && apt-get install pre-commit -y

COPY --from=uv --chown=vscode: /uv /uvx /bin/
