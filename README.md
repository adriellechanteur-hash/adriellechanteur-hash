# ADRIEL TMJ

### Builder · Agent infrastructure · TypeScript

```text
Agent = Model + Harness
```

Je construis des outils où le **modèle propose** et le **harnais prouve** : exécution contrôlée, permissions, receipts, sandboxes, land fail-closed.

I build control harnesses for coding agents — proof-carrying execution, not chat theater.

---

## Compétences

| Domaine | Stack |
| --- | --- |
| Langages | TypeScript (strict), Node.js ≥22, Python |
| Agent systems | Harness loops, ProofGate, receipts, LKG / recover |
| Sandboxes | Docker, Firecracker (Linux+KVM / WSL2) |
| Tooling | pnpm, Turborepo, Vitest, Biome, GitHub Actions |
| Observability | Audit JSONL, OTLP/HTTP logs & traces |
| Intégrations | MCP, OpenAI-compatible, Ollama, Anthropic |

`typescript` `nodejs` `ai-agents` `cli` `docker` `firecracker` `mcp` `otel` `github-actions`

---

## Projet phare — [HELIX](https://github.com/adrieltmj/HELIX)

**v0.3 READY** · MIT · [Release](https://github.com/adrieltmj/HELIX/releases/tag/v0.3.0) · [Readiness](https://github.com/adrieltmj/HELIX/blob/main/docs/reports/v0.3-readiness.md)

Harness de contrôle pour agents de programmation :

- Boucle autonome : propose → isolate → implement → verify → eval → LKG → land
- Sandboxes host / Docker / Firecracker one-shot
- Policy de promotion (humain par défaut, autonome opt-in)
- Probe CI `REMOTE_GREEN` · export OTLP

```bash
pnpm install && pnpm --filter @helix/cli build
node apps/cli/dist/main.js doctor
node apps/cli/dist/main.js run "hello" --provider mock
```

---

## En ce moment

- Affiner Helix (preuves ops, DX, surface produit)
- Agent harnesses & exécution vérifiable
- Ouvert aux échanges / collabs sur l'infra agents

---

## Contact

- GitHub : [@adrieltmj](https://github.com/adrieltmj)
- Projet : [HELIX](https://github.com/adrieltmj/HELIX)

---

### Stats

![GitHub stats](https://github-readme-stats.vercel.app/api?username=adrieltmj&show_icons=true&theme=tokyonight&hide_border=true)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=adrieltmj&layout=compact&theme=tokyonight&hide_border=true)

---

*Fail-closed by default. Proofs over promises.*
