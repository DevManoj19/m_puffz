# 🌟 m_puffz

Welcome to **m_puffz**, a decentralized web app deployed on the Internet Computer using DFINITY’s SDK. This project showcases a full-stack canister-based dApp featuring a Rust backend and a modern JavaScript frontend, seamlessly integrated on Web3 infrastructure.

---

## 🚀 Live on the Internet Computer

- 🌐 **Frontend (Main App):**  
  👉 [https://qqczw-maaaa-aaaaa-qanhq-cai.icp0.io](https://qqczw-maaaa-aaaaa-qanhq-cai.icp0.io)  
  📦 **Canister ID:** `qqczw-maaaa-aaaaa-qanhq-cai`

- 📡 **Backend (Candid Interface):**  
  👉 [https://a4gq6-oaaaa-aaaab-qaa4q-cai.raw.icpe.io/?id=qxd7c-byaaa-aaaaa-qanha-cai](https://a4gq6-oaaaa-aaaab-qaa4q-cai.raw.icpe.io/?id=qxd7c-byaaa-aaaaa-qanha-cai)  
  📦 **Canister ID:** `qxd7c-byaaa-aaaaa-qanha-cai`

---

## 📁 Project Structure

```

m\_puffz/
├── backend/              # Rust-based backend canister
│   ├── src/
│   ├── Cargo.toml
│   └── backend.did
├── frontend/             # JavaScript frontend (React/Vite/etc.)
│   ├── src/
│   └── package.json
├── dfx.json              # DFINITY configuration
├── README.md             # Project documentation
└── .gitignore

````

---

## 🧪 Run Locally

### Start Local Internet Computer Replica
```bash
dfx start --background
````

### Deploy Locally

```bash
dfx deploy
```

### Start Frontend (with Live Reload)

```bash
cd frontend
npm install
npm start
```

* Frontend: `http://localhost:8080`
* Replica: `http://localhost:4943`

---

## 🛰 Deploy to Mainnet

Make sure you're using your mainnet identity:

```bash
dfx identity use mainnet_id
dfx deploy --network ic
```

Check deployed canister status:

```bash
dfx canister --network ic status frontend
dfx canister --network ic status backend
```

---

## ⚙️ Environment Notes

* `npm run generate` — generates updated Candid bindings
* Set `DFX_NETWORK=ic` in production builds
* To avoid warnings, configure `.ic-assets.json5` with asset security policies

Example:

```json5
[
  {
    "match": "**/*",
    "security_policy": "strict"
  }
]
```

Or disable the warning:

```json5
{
  "disable_security_policy_warning": true
}
```

---

## 🔗 Resources

* [Internet Computer Developer Docs](https://internetcomputer.org/docs/current/developer-docs/)
* [Rust Canisters Guide](https://internetcomputer.org/docs/current/developer-docs/backend/rust/)
* [Candid Specification](https://internetcomputer.org/docs/current/developer-docs/backend/candid/)
* [ic-cdk Docs](https://docs.rs/ic-cdk)

---

## 👤 Author

* 🧑 GitHub: [DevManoj19](https://github.com/DevManoj19)
* 📦 Project Repo: [m\_puffz](https://github.com/DevManoj19/m_puffz)

---

## 📜 License

MIT License — feel free to fork, remix, and build on top of this project.

> Built with ❤️ using Rust, JavaScript, and DFINITY SDK on the Internet Computer 🌐

```
