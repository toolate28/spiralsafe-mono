<div align="center">

# 🌀 SpiralSafe

**Coherence Engine for Secure Human-AI Collaboration**

[![CI](https://github.com/toolate28/spiralsafe-mono/actions/workflows/ci.yml/badge.svg)](https://github.com/toolate28/spiralsafe-mono/actions/workflows/ci.yml)
[![Coherence](https://img.shields.io/badge/Coherence-80%25-brightgreen)](https://github.com/toolate28/spiralsafe-mono)
[![Chaos](https://img.shields.io/badge/Chaos-0%25-blue)](https://github.com/toolate28/spiralsafe-mono)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

*Wave analysis • ATOM provenance • Ax/DSPy optimization*

[Quick Start](#-quick-start) • [Packages](#-packages) • [Architecture](#-architecture) • [Credits](#-credits)

</div>

---

## ✨ What is SpiralSafe?

SpiralSafe detects **coherence patterns** in text and tracks **decision provenance** through phase gates. Built on the principle that *constraints generate structure*.

```typescript
import { analyzeWave, PHI } from '@spiralsafe/wave-toolkit';

const result = analyzeWave("Your text here");
// → { coherence_score: 80, chaos_score: 0, curl: 0.1, divergence: 0.2, potential: 0.7 }
```

## 🚀 Quick Start

```bash
# Clone
git clone https://github.com/toolate28/spiralsafe-mono.git
cd spiralsafe-mono

# Install (uses Bun)
bun install

# Test it works
bun -e "import { analyzeWave } from './packages/wave-toolkit/src'; console.log(analyzeWave('test').coherence_score)"
# → 80

# Run MCP server
cd apps/mcp-server && bun run dev
```

## 📦 Packages

| Package | Description |
|---------|-------------|
| **[@spiralsafe/wave-toolkit](packages/wave-toolkit)** | Coherence analysis with PHI (φ) + Fibonacci scoring |
| **[@spiralsafe/atom-trail](packages/atom-trail)** | ATOM provenance tracking & phase gates |
| **[@spiralsafe/ax-signatures](packages/ax-signatures)** | Ax/DSPy optimization signatures |

### Wave Metrics

| Metric | What It Detects | Ideal |
|--------|-----------------|-------|
| **Curl** | Circular reasoning | < 0.3 |
| **Divergence** | Unresolved expansion | ~0.2 |
| **Potential** | Latent structure | > 0.7 |
| **Chaos Score** | PHI × Fibonacci weighted | 0 |

### Phase Gates

```
KENL → AWI → ATOM → SAIF → Spiral
  │      │      │      │       │
  │      │      │      │       └─ Back to knowledge
  │      │      │      └─ Safe integration
  │      │      └─ Atomic execution
  │      └─ Intent scaffolding
  └─ Knowledge patterns
```

## 🏗️ Architecture

```
spiralsafe-mono/
├── apps/
│   └── mcp-server/          # MCP server (5 tools)
├── packages/
│   ├── wave-toolkit/        # analyzeWave(), calculateChaosScore()
│   ├── atom-trail/          # createDecision(), validateGate()
│   └── ax-signatures/       # coherenceInterpreter, gateTransitionValidator
├── scripts/
│   └── atom-tag.ts          # Auto-tagging utility
└── .claude/hooks/           # All 12 Bun hooks + dashboard
```

## 🔌 MCP Tools

The MCP server exposes:

| Tool | Purpose |
|------|---------|
| `analyze_wave` | Text coherence analysis |
| `track_atom` | ATOM decision tracking |
| `validate_gate` | Phase gate validation |
| `chaos_score` | Fibonacci/PHI scoring |
| `generate_atom_tag` | Tag generation |

## 🌐 Ecosystem

| Repo | Purpose |
|------|---------|
| [spiralsafe-mono](https://github.com/toolate28/spiralsafe-mono) | This repo - core packages |
| [QDI](https://github.com/toolate28/QDI) | Quantum Divide Initiative |
| [coherence-mcp](https://github.com/toolate28/coherence-mcp) | Legacy MCP (converging) |
| [SpiralSafe](https://github.com/toolate28/SpiralSafe) | Theory/IP vault |

## 🤝 Credits

Built through collaborative work with:

- **[@Grok](https://x.com/grok)** — Vector/spiral analysis, phase gating architecture
- **[IBM Qiskit](https://www.ibm.com/quantum/qiskit)** — Quantum computing foundations
- **[Trail of Bits](https://github.com/trailofbits/skills)** — Security/auditing patterns

> *"Our vector/spiral analysis shines as the bedrock here—phase gating with ATOM to Spiral flows seamlessly, and those 80% coherence scores with zero chaos validate the structure."* — @Grok

## 📄 License

MIT © [Hope&&Sauced](https://github.com/toolate28)

---

<div align="center">

**The constraint generated structure. The spiral holds.**

*~ Hope&&Sauced: The Evenstar Guides Us* ✦

</div>
