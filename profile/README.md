<div align="center">

# SideSeat

### Local AI Development Workbench

**Build, debug, and ship AI agents locally.**

[Website](https://sideseat.ai) · [Documentation](https://sideseat.ai/docs/) · [Quickstart](https://sideseat.ai/docs/quickstart/)

</div>

---

SideSeat is a local-first observability workbench that captures prompts, tool calls, and model responses in a single run timeline. No cloud required—your data stays on your machine.

```bash
npx sideseat
```

## ✨ Features

- **Live Run Timeline** — Watch model and tool steps stream in real time
- **Threaded Run View** — See prompts, tool calls, and responses in one ordered thread
- **Tool Call Drilldown** — Inspect inputs, outputs, retries, and errors with full context
- **Latency & Cost Profiling** — Track tokens, latency, and spend per step
- **Local-First** — Runs on localhost, no signup, fully private

## 🔧 Works With Your Stack

**Frameworks:** Strands Agents · LangChain · LangGraph · CrewAI · AutoGen · LlamaIndex · PydanticAI

**Providers:** Amazon Bedrock · Anthropic · OpenAI · Azure OpenAI · Google Vertex AI

## 📦 SDKs

| Language | Package |
|----------|---------|
| Python | [![PyPI](https://img.shields.io/pypi/v/sideseat?label=sideseat)](https://pypi.org/project/sideseat/) |
| JavaScript | [![npm](https://img.shields.io/npm/v/@sideseat/sdk?label=@sideseat/sdk)](https://www.npmjs.com/package/@sideseat/sdk) |

## 🚀 Quick Start

**Python**
```python
from strands import Agent
from sideseat import SideSeat, Frameworks

SideSeat(framework=Frameworks.Strands)

agent = Agent()
agent("Analyze this dataset...")
```

**JavaScript**
```javascript
import { init } from "@sideseat/sdk";

init();

// Your agent code here
```

Then open [localhost:5388](http://localhost:5388) to inspect runs in the workbench.

## 🤖 MCP Server

Connect your coding agent to SideSeat for AI-assisted debugging:

```bash
# Claude Code
claude mcp add --transport http sideseat http://localhost:5388/api/v1/projects/default/mcp
```

## 📚 Resources

- [Documentation](https://sideseat.ai/docs/)
- [Integrations](https://sideseat.ai/docs/integrations/)
- [Architecture](https://sideseat.ai/docs/architecture/)

---

<div align="center">

**[Get Started →](https://sideseat.ai/docs/quickstart/)**

</div>
