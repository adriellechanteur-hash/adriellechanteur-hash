# ADRIEL TMJ

### Builder · Agent infrastructure · TypeScript

<p align="left">
  <a href="https://github.com/adrieltmj/HELIX"><img src="https://img.shields.io/badge/Project-HELIX-0A7A5A?style=for-the-badge&logo=github" alt="HELIX" /></a>
  <a href="https://github.com/adrieltmj/HELIX/releases/tag/v0.3.0"><img src="https://img.shields.io/badge/v0.3-READY-1F6FEB?style=for-the-badge" alt="v0.3" /></a>
  <a href="https://github.com/adrieltmj/HELIX/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="MIT" /></a>
</p>

```text
Agent = Model + Harness
```

Je construis des outils où le **modèle propose** et le **harnais prouve** : exécution contrôlée, permissions, receipts, sandboxes, land fail-closed.

I build **control harnesses for coding agents** — proof-carrying execution, not chat theater.

---

## Qui je suis

- **Focus** : infrastructure pour agents de code (harness, preuves, sandboxes)
- **Style** : fail-closed, TDD, ADR, preuves d'environnement avant les slogans
- **Langues** : Français · English
- **Dispo** : ouvert aux collabs / retours sur Helix et l'infra agents

---

## Compétences

| Domaine | Stack |
| --- | --- |
| Langages | TypeScript (strict), Node.js ≥22, Python |
| Agent systems | Harness loops, ProofGate, receipts, LKG / recover / land |
| Sandboxes | Host · Docker · Firecracker (Linux+KVM / WSL2) |
| Tooling | pnpm · Turborepo · Vitest · Biome · GitHub Actions |
| Observability | Audit JSONL · OTLP/HTTP logs & traces |
| Intégrations | MCP · OpenAI-compatible · Ollama · Anthropic |

<p>
  <img src="https://img.shields.io/badge/TypeScript-strict-3178C6?logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Node.js-22+-339933?logo=nodedotjs&logoColor=white" alt="Node" />
  <img src="https://img.shields.io/badge/AI%20Agents-harness-6E40C9" alt="Agents" />
  <img src="https://img.shields.io/badge/Docker-sandbox-2496ED?logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Firecracker-microVM-FF9900" alt="Firecracker" />
  <img src="https://img.shields.io/badge/MCP-tools-000000" alt="MCP" />
  <img src="https://img.shields.io/badge/OTLP-observability-FF6B35" alt="OTLP" />
</p>

---

## Projet phare — [HELIX](https://github.com/adrieltmj/HELIX)

**Control harness for coding agents** · [v0.3 readiness](https://github.com/adrieltmj/HELIX/blob/main/docs/reports/v0.3-readiness.md) · [Release v0.3.0](https://github.com/adrieltmj/HELIX/releases/tag/v0.3.0)

| Capacité | Rôle |
| --- | --- |
| ProofGate + receipts | Une commande n'est vraie que si hashée et vérifiable |
| Autonomous loop | propose → isolate → implement → verify → eval → LKG → land |
| Sandboxes | host / Docker / Firecracker one-shot |
| Policy | humain `--approve` par défaut · autonome opt-in |
| CI probe | `helix ci remote-status` → `REMOTE_GREEN` |
| OTel | export logs + traces OTLP/HTTP |

```bash
pnpm install && pnpm --filter @helix/cli build
node apps/cli/dist/main.js doctor
node apps/cli/dist/main.js run "hello" --provider mock
node apps/cli/dist/main.js verify --command node --arg -e --arg "process.exit(0)" --claim "command succeeded"
```

[![CI](https://github.com/adrieltmj/HELIX/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/adrieltmj/HELIX/actions/workflows/ci.yml)

---

## Ce que je cherche / offre

- Retours d'utilisateurs et contributeurs sur Helix
- Discussions autour des **agent harnesses**, sandboxes, preuve d'exécution
- Partage d'expériences fail-closed / ProofGate-like systems

---

## En ce moment

- Affiner Helix (DX, preuves ops, surface produit)
- Documenter les boucles agent ↔ harness
- Rendre le profil et le dépôt plus découvrables

---

## Contact

- GitHub : [@adrieltmj](https://github.com/adrieltmj)
- Helix : [github.com/adrieltmj/HELIX](https://github.com/adrieltmj/HELIX)
- Issues / discussions bienvenues sur le dépôt

---

### Stats

![GitHub stats](https://github-readme-stats.vercel.app/api?username=adrieltmj&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=adrieltmj&layout=compact&theme=tokyonight&hide_border=true)
![Streak](https://streak-stats.demolab.com/?user=adrieltmj&theme=tokyonight&hide_border=true)

---

*Fail-closed by default. Proofs over promises.*
