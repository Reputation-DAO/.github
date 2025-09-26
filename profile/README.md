
<h1 align="center">Reputation DAO</h1>
<p align="center">
  Soulbound, tamper-proof reputation for the Internet Computer (ICP).<br/>
  Factory-managed multitenancy, configurable decay, and full on-chain auditability.
</p>

<p align="center">
  <a href="https://37le5-2yaaa-aaaam-qdwhq-cai.icp0.io/"><b>App</b></a> •
  <a href="https://github.com/Reputation-DAO/Reputation-DAO">Core Repo</a> •
  <a href="https://github.com/Reputation-DAO/RepDao-Cli">CLI / JS SDK</a> •
  <a href="https://x.com/Reputation_Dao">X</a> •
  <a href="https://t.me/reputationdao">Telegram</a> •
  <a href="https://www.youtube.com/watch?v=iaZ4pHaWd_U">Demo</a>
</p>

---

## ✨ What we’re building

* **Soulbound reputation** bound to principals — non-transferable by design
* **Decay engine** (rate, interval, thresholds, grace) to keep scores fresh
* **Factory–pool architecture** to mint, assign, upgrade, recycle per-org canisters
* **Auditable events & analytics**: leaderboard, awarder stats, org pulse, history
* **Modern UX**: React/Vite, Tailwind + shadcn/ui, connect2ic (Plug, Stoic, II)

## 🧱 Architecture (high-level)

* **Factory canister** — owns canonical child WASM, tops up cycles, assigns orgs, handles upgrades & recycling
* **Child reputation canister** — per-org actor with mint/revoke, limits, blacklist, decay, analytics
* **Blog backend** — lightweight CMS canister for the frontend’s blog/docs updates
* **Frontend** — role-aware dashboards, docs, and community pages

## 📦 Repositories

* **Core:** [`Reputation-DAO`](https://github.com/Reputation-DAO/Reputation-DAO) — Motoko canisters + React/Vite app
* **CLI / SDK:** [`RepDao-Cli`](https://github.com/Reputation-DAO/RepDao-Cli) — global CLI + JS/TS client

## 🚀 Quick start (local)

```bash
git clone https://github.com/Reputation-DAO/Reputation-DAO
cd Reputation-DAO

# start IC local replica
dfx start --background --clean

# deploy canisters (factory, child template, blog backend, frontend)
dfx deploy --network local

# run frontend
cd frontend && npm install && npm run dev
# open http://localhost:5173 and connect Plug / Stoic / II
```

## 🛡️ Security

See **SECURITY.md** for our disclosure workflow and supported releases.
Report vulnerabilities: **[security@reputationdao.dev](mailto:security@reputationdao.dev)**

## 🤝 Contributing

Open an issue with `backend`, `frontend`, `docs`, or `community` labels.
PRs welcome — please include impact/ops notes (cycles, env updates).

---

<p align="center">
  <i>Built on ICP • © 2025 Reputation DAO</i>
</p>
