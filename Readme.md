# 🤖 Cagent Comedy Central 🤖

> A lighthearted, multi-agent AI playground—where agents collaborate, delegate, and sometimes crack a joke or two! Powered by [cagent](https://github.com/artofthepossible/cagent-comedy-central).

---

## 🎭 About

Cagent Comedy Central is your launchpad for experimenting with multi-agent AI workflows. Build, run, and orchestrate teams of specialized AI agents—each with their own skills, tools, and personalities—all from a simple YAML file. Whether you want a helpful assistant, a code reviewer, or a stand-up comedian, cagent makes it easy (and fun) to get started.

---

## 🛠️ Tech Stack

- **cagent** (multi-agent runtime)
- **YAML** (agent configuration)
- **Docker** (optional, for MCP tool servers)
- **OpenAI / Anthropic / Gemini / DMR** (AI model providers)

---

## � Prerequisites

- Prebuilt binaries for Windows, macOS and Linux can be found on the releases page of the [project's GitHub repository](https://github.com/docker/cagent/releases)


- (Optional) [Docker Desktop](https://www.docker.com/products/docker-desktop) for running MCP tool servers
- API keys for your preferred AI provider (OpenAI, Anthropic, Gemini, or DMR)

---

## 🚀 Quick Start

### 1. Download & Install

Download the prebuilt binary for your platform from the [cagent releases page](https://github.com/docker/cagent/releases).

On macOS/Linux, make it executable:

```bash
chmod +x /path/to/cagent-binary
```

### 2. Set Your API Keys

```bash
# For OpenAI
export OPENAI_API_KEY=your_api_key_here
# For Anthropic
export ANTHROPIC_API_KEY=your_api_key_here
# For Gemini
export GOOGLE_API_KEY=your_api_key_here
```

### 3. Run Your First Agent

```bash
./cagent run container-nerdy-central.yaml --debug
```

Or try generating a new agent/team interactively:

```bash
./cagent new
```

---

## 🎯 Key Features

- 🏗️ **Multi-agent architecture** – Compose teams of agents for different domains
- 🔧 **Rich tool ecosystem** – Integrate external tools/APIs via MCP protocol
- 🤝 **Smart delegation** – Agents can route tasks to the best specialist
- 📝 **YAML configuration** – Declarative, human-friendly agent setup
- 💭 **Advanced reasoning** – Built-in "think", "todo", and "memory" tools
- 🌐 **Multiple AI providers** – OpenAI, Anthropic, Gemini, DMR (Docker Model Runner)

---

## 🏃 Example Usage

Run an agent from your YAML config:

```bash
./cagent run container-nerdy-central.yaml --debug
```

Generate a new agent or team with a single prompt:

```bash
./cagent new --model openai/gpt-5-mini --max-tokens 32000
```

Push your agent to Docker Hub:

```bash
./cagent push ./container-nerdy-central.yaml yourdockeruser/cagent-comedy-central
```

Pull an agent from Docker Hub:

```bash
./cagent pull yourdockeruser/cagent-comedy-central
```

---

## � More Resources

- [Full Usage Guide](https://github.com/artofthepossible/cagent/blob/main/docs/USAGE.md)
- [Agent Examples](https://github.com/artofthepossible/cagent/tree/main/examples)
- [MCP Toolkit & Catalog](https://docs.docker.com/ai/mcp-catalog-and-toolkit/toolkit/)


---

## 💡 Getting Help

For command help:

```bash
./cagent --help
./cagent [command] --help
```

For feedback or issues:

```bash
./cagent feedback
```



---

Made with 🤖, YAML, and a dash of humor!