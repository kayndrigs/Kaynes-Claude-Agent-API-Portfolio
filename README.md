# Kayne's Claude Bedrock API Portfolio

Hands-on explorations of the Claude ecosystem — API fundamentals, prompting & tool use, Claude Code workflows, and Model Context Protocol basics.

## Structure

```
notebooks/   Jupyter notebooks — runnable end-to-end examples
diagrams/    PlantUML architecture and system design diagrams
docs/        Supporting reference material
```

## Notebooks

| Notebook | Domain | Description |
|----------|--------|-------------|
| [claude_agent_definitions.ipynb](notebooks/claude_agent_definitions.ipynb) | Claude API fundamentals | Explore `AgentDefinitions` in the Claude Agent SDK — how agents are declared, configured, and invoked |
| [hub_spoke_bedrock.ipynb](notebooks/hub_spoke_bedrock.ipynb) | Claude API fundamentals | Hub-and-spoke multi-agent architecture on AWS Bedrock using the Converse API (ap-southeast-1, Claude Sonnet 4.6) |
| [financial_resolution_agent.ipynb](notebooks/financial_resolution_agent.ipynb) | Prompting & tool use · MCP basics | Financial resolution agent with a full tool registry, MCP integration, and hooks-driven orchestration |
| [stop_reason_demo.ipynb](notebooks/stop_reason_demo.ipynb) | Claude API fundamentals | Understanding `stop_reason` values from Claude on AWS Bedrock and what each one signals about model behavior |

## Diagrams

| Diagram | Description |
|---------|-------------|
| [claude_agent_definitions.puml](diagrams/claude_agent_definitions.puml) | Component diagram of the Claude Agent SDK's agent definition model |
| [agent_definitions_demo.puml](diagrams/agent_definitions_demo.puml) | Sequence diagram for the agent definitions demo flow |
| [hub_spoke_bedrock.puml](diagrams/hub_spoke_bedrock.puml) | Hub-and-spoke multi-agent topology on Bedrock |
| [context_passing_strategy.puml](diagrams/context_passing_strategy.puml) | Strategies for passing context between agents |
| [animal_chess/](diagrams/animal_chess/) | Class diagrams for an Animal Chess (Jungle Chess) MCO1 project |
| [claims/](diagrams/claims/) | Claim source and precedent flow diagrams |

## Prerequisites

```bash
pip install anthropic boto3 python-dotenv rich
```

AWS credentials configured for Bedrock notebooks (`ap-southeast-1`).

## Domains Covered

- **Claude API fundamentals** — SDK setup, agent definitions, stop reasons, Bedrock Converse API
- **Prompting & tool use** — structured tool registries, hook-driven control flow
- **Claude Code workflows** — multi-agent orchestration patterns
- **Model Context Protocol basics** — MCP tool integration in the financial agent
