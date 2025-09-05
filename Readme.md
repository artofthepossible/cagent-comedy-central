# Cagent Quick Start Guide

Cagent is a command-line tool for running AI agents with a simple and intuitive interface.

## 🚀 Installation

### Download Binary
Download the prebuilt binary for your platform from the [releases page](https://github.com/your-project/cagent/releases) of the project's GitHub repository.

### Set Executable Permissions
On macOS and Linux, make the binary executable:

```bash
chmod +x /path/to/cagent-binary
```

Example:
```bash
chmod +x /{Home}/apps/goldenpath/cagent-bin/cagent-darwin-arm64
```

## ✅ Verify Installation

Check that cagent is working properly:

```bash
./bin/cagent --version
./bin/cagent --help
```

## 📋 Available Commands

Cagent provides several commands for managing and running AI agents:

| Command | Description |
|---------|-------------|
| `api` | Start the API server |
| `catalog` | Manage the agent catalog |
| `exec` | Execute an agent |
| `new` | Create a new agent configuration |
| `pull` | Pull an artifact from Docker Hub |
| `push` | Push an artifact to an OCI registry |
| `readme` | Print the README of an agent |
| `run` | Run an agent |
| `version` | Print version information |

## 🏃 Running Your First Agent

To run an agent, use the `run` command with a path to your agent configuration file:

```bash
./bin/cagent run /path/to/your/agent.yaml --debug
```

Example:
```bash
./bin/cagent run /{Home}//path/to/your/agent/container-nerdy-central.yaml --debug
```

## 🚩 Global Flags

- `-d, --debug`: Enable debug logging
- `-h, --help`: Show help information
- `-o, --otel`: Enable OpenTelemetry tracing

## 💡 Getting Help

For detailed information about any command:

```bash
cagent [command] --help
```

For general help:
```bash
cagent --help
```

## 🔧 Feedback

Have feedback or issues? Use the feedback command:

```bash
cagent feedback
```

---

**Ready to get started?** Download cagent, make it executable, and run your first agent!