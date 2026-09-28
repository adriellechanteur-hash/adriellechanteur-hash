# ADRIEL TMJ

### Builder Â· Agent infrastructure Â· TypeScript

```text
Agent = Model + Harness
```

Je construis des outils oÃ¹ le **modÃ¨le propose** et le **harnais prouve** : exÃ©cution contrÃ´lÃ©e, permissions, receipts, sandboxes, land fail-closed.

ðŸ‡¬ðŸ‡§ *I build control harnesses for coding agents â€” proof-carrying execution, not chat theater.*

---

## CompÃ©tences

| Domaine | Stack |
| --- | --- |
| Langages | TypeScript (strict), Node.js â‰¥22, Python |
| Agent systems | Harness loops, ProofGate, receipts, LKG / recover |
| Sandboxes | Docker, Firecracker (Linux+KVM / WSL2) |
| Tooling | pnpm, Turborepo, Vitest, Biome, GitHub Actions |
| Observability | Audit JSONL, OTLP/HTTP logs & traces |
| IntÃ©grations | MCP, OpenAI-compatible, Ollama, Anthropic |

`typescript` `nodejs` `ai-agents` `cli` `docker` `firecracker` `mcp` `otel` `github-actions`

---

## Projet phare â€” [HELIX](https://github.com/adriellechanteur-hash/HELIX)

**v0.3 READY** Â· MIT Â· [Release](https://github.com/adriellechanteur-hash/HELIX/releases/tag/v0.3.0) Â· [Readiness](https://github.com/adriellechanteur-hash/HELIX/blob/main/docs/reports/v0.3-readiness.md)

Harness de contrÃ´le pour agents de programmation :

- Boucle autonome : propose â†’ isolate â†’ implement â†’ verify â†’ eval â†’ LKG â†’ land
- Sandboxes host / Docker / Firecracker one-shot
- Policy de promotion (humain par dÃ©faut, autonome opt-in)
- Probe CI `REMOTE_GREEN` Â· export OTLP

```bash
pnpm install && pnpm --filter @helix/cli build
node apps/cli/dist/main.js doctor
node apps/cli/dist/main.js run "hello" --provider mock
```

---

## En ce moment

- Affiner Helix (preuves ops, DX, surface produit)
- Agent harnesses & exÃ©cution vÃ©rifiable
- Ouvert aux Ã©changes / collabs sur lâ€™infra agents

---

## Contact

- GitHub : [@adriellechanteur-hash](https://github.com/adriellechanteur-hash)
- Projet : [HELIX](https://github.com/adriellechanteur-hash/HELIX)
- Prefer handle (rename en cours) : **`adrieltmj-hash`**

---

### Stats

![GitHub stats](https://github-readme-stats.vercel.app/api?username=adriellechanteur-hash&show_icons=true&theme=tokyonight&hide_border=true&count_private=true)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=adriellechanteur-hash&layout=compact&theme=tokyonight&hide_border=true)

---

*Fail-closed by default. Proofs over promises.*
