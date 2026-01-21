# Claude Code Sub-Agents

A collection of specialized Claude sub-agents organized by category. Each sub-agent is designed to handle specific tasks with domain expertise.

## Categories

### Security

- **[brinqa-vuln-assessor](brinqa-vulnerability-assessor/)** - Analyzes Brinqa security findings and determines remediation actions

---

## How to Use Sub-Agents

Sub-agents are invoked using the Task tool with the appropriate `subagent_type`. Each sub-agent folder contains:

1. **agent.md** - Instructions and decision-making logic for the agent
2. **EXAMPLES.md** (optional) - Real-world examples demonstrating capabilities

Example: To use the Brinqa vulnerability assessor, call the Task tool with `subagent_type="brinqa-vuln-assessor"`.

## Contributing

To add a new sub-agent:

1. Create a folder at the root level: `agent-name/`
2. Add the required `agent.md` file with detailed instructions
3. Optionally add `EXAMPLES.md` with usage examples
4. Update this README.md under the appropriate category with a one-liner description