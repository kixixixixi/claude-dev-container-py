FROM node:24-alpine

COPY --from=ghcr.io/astral-sh/uv:latest /uv /uvx /usr/local/bin/

RUN apk add --no-cache \
    git \
    bash \
    curl

RUN npm install -g @anthropic-ai/claude-code

WORKDIR /workspace
