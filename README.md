# docker-compose-fabric-ai
Use `fabric-ai`'s `REST API` and `MCP server` inside `Docker` containers and manage with `docker compose`

Special thanks to:
- @danielmiessler, @ksylvan, creators of `fabric-ai` and `fabric-mcp`!
- @jimscard for teaching me everything I know about this and witnessing my learning process!

## Repository links:

- [`fabric-ai`](https://github.com/danielmiessler/Fabric.git) @danielmiessler ultimate repository
	- Also [here](https://github.com/ksylvan/fabric.git)
- [`fabric-mcp`](https://github.com/ksylvan/fabric-mcp.git) @ksylvan fabric-mcp
- [`fabric-mcp`](https://github.com/jimscard/fabric-mcp.git) @jimscard fork for use in Docker
	- See also: ["Start / stop / use a containerized instance of fabric"](https://github.com/jimscard/fabric-d.git)

## Docker images

- [`kayvan/fabric`](https://hub.docker.com/r/kayvan/fabric)
	- or `docker pull kayvan/fabric:latest`
- [`jimscard/fabric-yt`](https://hub.docker.com/r/jimscard/fabric-yt)
	- or `docker pull jimscard/fabric-yt:latest`

# Purpose

Fabric is already an amazing tool for maximizing and optimizing the use of AI through the Fabric CLI. This is taken even further when given as tools for an LLM itself. The goal is to utilize these tools safely through in containers, via Docker.

It can become quite a hassle to have to manage your fabric server REST API instance along with configuring the MCP server. While it technically is easier to set it and forget, there are some noticeable improvements:

1. We run a fabric server inside a docker container, not on your local machine. This is also where the fabric magic happens,
2. We run the fabric MCP server inside a docker container, not on your local machine; this significantly improves security, and is generally still the best practice with MCP servers.
3. Managing the REST API and MCP server with `docker compose` makes building, starting, and stopping a breeze; everything is connected within a docker network as well.

In this repo, I will guide you through the installation process, configuration, and usage, along with all the technical details.

# Installation

## Simple Installation

### Requirements

## Manual Installation (more freedom and customization)

### Requirements

# Usage

### All examples will be using:
- [LM Studio](https://lmstudio.ai) as the MCP client
- [Cerebras AI](https://www.cerebras.ai) as fabric's vendor

## Adjustments

# Extra helpful resources

- [Git cloning CLI tool for automated organization of repositories](https://github.com/grdl/git-get)
- [Cool docker engine monitoring CLI tool](https://github.com/jesseduffield/lazydocker.git)
