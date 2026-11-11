### Hi, I'm Ahmed (Eli)

I build software with AI coding agents, and the tooling that lets several of them work in one repository without breaking each other.

Software & AI Engineer at [DPA+](https://dpa.plus) in Munich · CS at TU München

#### Open source

- **[comms](https://github.com/dpa-plus/comms)**: coordination layer for parallel coding agents (Claude Code, Codex). An agent claims a file before it edits, everything lands in one append-only log, and a git hook refuses a commit that would take another agent's work. Also runs as an MCP server. Go + Python.
- **[satz](https://github.com/dpa-plus/satz)**: dictation app for macOS, Windows and Linux. Double-tap a key, speak, and the text appears where your cursor is. Bring your own model or run Whisper locally. Swift + Electron. [dpa.plus/satz](https://dpa.plus/satz/)
- **[antigravity-plugin-cc](https://github.com/dpa-plus/antigravity-plugin-cc)**: Gemini as a second reviewer inside Claude Code: review, adversarial review and delegated tasks.
- **[request-interceptor](https://github.com/dpa-plus/request-interceptor)**: hooks into requests and AI prompts for analysis, modification and observability.

#### How I work

- Several agents in parallel on one repo, coordinated through comms. One agent does a task, a different one verifies it.
- A second model reviews what the first one wrote before it ships.
- Proof before trust: benchmarks on sealed, held-out test sets with hidden twins to catch overfitting, hill-climbed round after round, and core logic formally verified in Dafny where a mistake would be expensive.
- The unglamorous parts stay non-negotiable: tests, type checks, auth, tenant isolation.

Most of my day job lives in private client repositories: full-stack TypeScript (Next.js, Node, Prisma, Postgres) with LLM features in production.

[LinkedIn](https://www.linkedin.com/in/ahmed-elnaghi)
