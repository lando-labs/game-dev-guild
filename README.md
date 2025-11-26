# Game Dev Guild

**A CAMI Agent Collection for Phaser 3 Game Development**

> **Status: Experimental**
> These agents are newly created and minimally tested. They serve as an example of how to build a specialized agent guild using CAMI and agent-architect.

## What is This?

This is an example "agent guild" - a collection of specialized Claude Code agents designed to work together on a specific domain. In this case: **2D web game development with Phaser 3**.

These agents were created entirely through CAMI's agent-architect, demonstrating how you can rapidly build a team of AI specialists tailored to your tech stack and workflows.

## Agents in This Guild

| Agent | Class | Purpose |
|-------|-------|---------|
| **phaser-core** | Technology Implementer | Core Phaser 3 - scenes, sprites, physics, input, cameras, tweens |
| **level-designer** | Technology Implementer | Tiled integration, tilemaps, collision layers, world building |
| **game-systems** | Technology Implementer | Inventory, dialogue, save/load, state machines, quests, scoring |
| **mcp-architect** | Strategic Planner | MCP server design - tool APIs, architecture decisions |
| **game-qa** | Technology Implementer | Game testing - performance, visual regression, cross-browser |
| **audio-specialist** | Technology Implementer | Sound effects, music, spatial audio, Web Audio API |
| **ui-specialist** | Technology Implementer | HUD, menus, health bars, responsive game UI |
| **ai-behaviors** | Technology Implementer | Enemy AI, pathfinding, behavior trees, state machines |

## Tech Stack Focus

See `STRATEGIES.yaml` for the full tech stack, but highlights include:

- **Phaser 3.80+** - Primary game engine
- **TypeScript 5+** - Type-safe game code
- **Vite 5+** - Fast development builds
- **Tiled Map Editor** - Level design
- **Vitest + Playwright** - Testing

## How These Agents Were Created

1. Created a new CAMI source directory for the guild
2. Defined the tech stack and strategies in `STRATEGIES.yaml`
3. Used agent-architect to generate each specialist agent in parallel
4. Each agent follows the three-class system (Workflow Specialist, Technology Implementer, Strategic Planner)

## Using This Guild

### With CAMI

```bash
# Add this source to your CAMI config
cami source add <git-url>

# Deploy agents to your game project
cami deploy phaser-core level-designer game-qa ~/my-game
```

### Manual

Copy the `.md` agent files you need to your project's `.claude/agents/` directory.

## Contributing

These agents are experimental! If you use them and find issues or improvements:

1. Test the agent on real game development tasks
2. Note what works well and what doesn't
3. Submit issues or PRs with specific feedback

## License

MIT - Use freely, improve openly.

---

*Built with [CAMI](https://github.com/lando-labs/cami) - Claude Agent Management Interface*
