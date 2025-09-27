
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

---

## 🧠 Project Concept

Reputation DAO is a **soulbound, on-chain trust layer** built with Motoko on ICP.  
It enables any community, DAO, or organization to **issue, track, and manage reputation** transparently:

- Members earn rep for **valuable, provable contributions**.  
- Reputation is **non-transferable** (“soulbound”) and stays with the identity.  
- **Optional recovery logic** exists for compromised wallets.  
- **Freshness factor** ensures reputation remains relevant over time:  



repWeight = baseRep * freshnessFactor



All activity is **fully on-chain and publicly verifiable**.

---

## 🔄 Applications

1. 🌐 **Online Communities** — reward helpful posts, replies, or verified contributions.  
2. 💼 **Professional Networks** — freelancers & teams showcase credibility with on-chain proof.  
3. 🧑‍💻 **Open Source & DAOs** — PRs, bounties, governance votes tied to reputation.  
4. 🎓 **Education & Credentials** — verified skills, badges, and course completions as portable rep.  

---

## 📜 Key Rules

- **Soulbound:** rep cannot be transferred  
- **Controlled minting:** only trusted awarders can assign  
- **Daily mint limits:** prevents abuse/inflation  
- **Revocation:** admins/system can revoke fake or farmed rep  
- **Public ledger:** open, auditable, tamper-proof  

---

## 🧱 Architecture (high-level)

* **Factory canister** — manages canonical WASM, pools, upgrades, cycle top-ups  
* **Child reputation canister** — per-org actor with mint/revoke, decay, analytics, blacklists  
* **Blog backend** — lightweight CMS for docs/community content  
* **Frontend** — role-aware dashboards, docs, and community pages  

---

## 📦 Repositories

* **Core:** [`Reputation-DAO`](https://github.com/Reputation-DAO/Reputation-DAO) — Motoko canisters + React/Vite app  
* **CLI / SDK:** [`RepDao-Cli`](https://github.com/Reputation-DAO/RepDao-Cli) — global CLI + JS/TS client  

---

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
````

---

## 🛡️ Security

See **SECURITY.md** for disclosure workflow & supported releases.
Report vulnerabilities: **[security@reputationdao.dev](mailto:security@reputationdao.dev)**

---

## 🤝 Contributing

Open an issue with `backend`, `frontend`, `docs`, or `community` labels.
PRs welcome — please include notes on **cycles/ops impact**.

---

<p align="center">
  <i>Built on ICP • © 2025 Reputation DAO</i>
</p>
```

This keeps your **current org README style** intact, but folds in the **expanded repo description (concept, rules, use cases)** you showed me.

Want me to also refine the **Quickstart** into a separate “Playground Deploy” section (like your repo’s step-by-step with `dfx deploy --network playground` and Plug ID setup), so contributors can test faster without going local?
