# Claude Code Sub-Agents

A collection of specialized Claude sub-agents organized by category. Each sub-agent is designed to handle specific tasks with domain expertise.

## Categories

### Security

Security-focused agents for vulnerability management, security assessments, and remediation.

#### Brinqa Vulnerability Manager

**Purpose:** Assesses security vulnerabilities from the Brinqa system and determines appropriate remediation actions.

**Capabilities:**
- Analyzes vulnerabilities from SkiShield code scanning and penetration testing
- Evaluates codebase impact and exploitability
- Determines whether to fix immediately, request risk exception, mark as not actionable, or accept risk
- Generates comprehensive exception and acceptance request documents

**When to Use:**
- When you receive vulnerability findings from the Brinqa system
- To assess the impact of CVEs on your codebase
- To determine the appropriate remediation strategy
- To generate risk exception or acceptance requests

**Location:** [security/brinqa-vulnerability-manager](security/brinqa-vulnerability-manager/)

---

## How to Use Sub-Agents

Sub-agents are specialized Claude instances that you can invoke to handle specific tasks. Each sub-agent has:

1. **README.md** - Overview, capabilities, and usage instructions
2. **agent.md** - Detailed instructions and decision-making logic for the agent
3. **EXAMPLES.md** - Real-world examples demonstrating the agent's capabilities

To use a sub-agent, provide it with the relevant context and let it analyze and respond according to its specialized knowledge.

## Contributing

To add a new sub-agent:

1. Create a category folder if it doesn't exist
2. Create a subfolder for your agent: `category/agent-name/`
3. Add the required files: `README.md`, `agent.md`, and `EXAMPLES.md`
4. Update this root README.md with your agent's details