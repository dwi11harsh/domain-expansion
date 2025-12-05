# domain-expansion

it is what it sound like, this won't define what your domain is (a fully blown coding agent) this is just meant to increase your domain and act as helping agent, but you need to be the one defining what the domain is

## What is this?

An interactive coding assistant powered by Qwen (via Ollama Cloud) that solves programming problems through natural conversation. Unlike your typical "move fast and break things" AI, this one has the audacity to ask for permission before running commands.

## Features that am thinking or rn (might CRUD these later)

- **Human-in-the-loop**: Every command requires your approval. Yes, even `ls`.
- **Streaming responses**: Watch the AI think in real-time (or don't, it's collapsible).
- **Strategy switching**: When the agent gets stuck, a meta-agent steps in and tries a different approach. Because sometimes the third time's not the charm.
- **Isolated thinking**: The agent's chain-of-thought doesn't pollute the conversation. (I mean why should it)
- **State persistence**: Crash? No problem. Resume exactly where you left off.
- **Rich TUI**: Because terminal UIs don't have to look like they're from 1985 and yet they need to seem cool to us coders.

## Installation

just clone it

## Quick Start

1. Set up your `.env` file:

   ```bash
   OLLAMA_URL=http://your-ollama-cloud-url
   MODEL=qwen
   ```

2. Run it:

   ```bash
   domain-expansion
   ```

3. Tell it what to do. It'll ask before doing anything. not a promise.

## How It Works

1. You describe a problem or task
2. Agent thinks about it (you can peek at the thinking if you're curious)
3. Agent wants to run a command → shows you what it wants to do
4. You approve/reject (you're in control, boss)
5. Command runs → results go back to agent
6. Repeat until solved or you get bored

If the agent tries the same thing 3 times and fails, a meta-agent steps in and tries a completely different strategy. Because doing the same thing and expecting different results is... well, you have tried relationships.

## Configuration

Everything goes in `.env`. Because environment variables are the adult way to do configuration. Fight me.

- `OLLAMA_URL`: Your Ollama Cloud endpoint
- `MODEL`: Model name (defaults to `qwen`)
- `LOG_LEVEL`: How chatty you want the logs (defaults to `verbose`)

## Why "domain-expansion"?

Because expanding your coding domain sounds cooler than "yet-another-cli-agent". Also, it's a reference that exactly 47% of developers will get. You know who you are.

## Contributing

PRs welcome. Tests appreciated. Documentation... please bro, I might get it but I promise others won't.

## License

MIT. Do whatever. Just don't blame me when the AI suggests `rm -rf /`.

---

_Built with questionable amounts of coffee, some song on infinite repeat and the naive belief that AI can code in a way that `I` like._
