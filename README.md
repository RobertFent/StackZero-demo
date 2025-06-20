![StackZero Frozen Icon](stackzero.png)

# StackZero Demo

This is the **public demo** of StackZero — a minimal, production-ready SaaS boilerplate you can self-host for just ~5€/month.

💡 Looking to launch your own SaaS? I offer a full setup service that includes:
- VPS & domain setup
- Secure deployment
- Private backend logic
- 🚀 Demo URL: [https://robertfent.com](https://robertfent.com)
- 👉 [Get started on Fiverr](http://www.fiverr.com/s/qD36b55)

## 🌱 What is StackZero?

StackZero is a lightweight SaaS starter kit built with:

- ✅ HTMX frontend (no JavaScript frameworks)
- ✅ Docker-based single-container deployment
- ✅ SQLite database with migrations
- ✅ Simple routing and templating structure
- ✅ < 5€/month to run (Hetzner + IONOS)

  
This repo includes the **frontend template and example routes**.

> 💡 The full business logic (`core/`) and internal backend modules are part of the private StackZero image — available via setup service.


## 🌱 Philosophy

- 💡 **Zero Stack Bloat** — No frontend frameworks, no TypeScript, no fancy build tools.
- 🧩 **Modular Backend** — All logic lives in `core`, maintained privately.
- 🖼️ **Template Frontend** — A generic `app` folder you can override entirely.
- 🚀 **Simple Deployment** — One `docker-compose.yml` and you're live.
- 💸 **5€ SaaS-Ready** — Designed to run on a 4€ Hetzner VPS + 1€ domain.


## 🔧 Design Principles

- No transpilers: Plain JavaScript (ES Modules), no TypeScript.
- No build step: Static assets served directly.
- No frontend framework: Uses htmx and a custom html.js parser.
- Single process: No multi-service architecture, everything runs in one container.
- Portable: Works on amd64 and arm64 thanks to multi-arch Docker builds.


## 🧠 Core Logic (Private)

The full backend logic (templating engine, routing, DB layer, etc.) is part of the private StackZero core.

This demo includes only the frontend template, example routes, and views.  
To get full access and deployment support, check out the [setup service](https://www.fiverr.com/s/gDwXyZv).


## 🔒 Security & Isolation

- Users can override the app/ folder via Docker but cannot access core/
- The core logic is mounted in the image, not the host – source code stays private
- Only a thin public interface (e.g., core_api.js) is exposed to the user app, if needed - feature not supported yet


## 🧰 Minimal Deployment Stack

StackZero is designed to run on:
| Component | Cost |
|---------------|--------------|
| Hetzner VPS | ~4.00 € /mo |
| Domain | ~1.00 € /mo |
| **Total** | **5.00 €** |

Perfect for small tools, prototypes, or self-hosted SaaS products.


## 📦 Example Use Cases

- Internal dashboards
- Lightweight SaaS apps
- Microtools with login/auth
- Self-hosted CRUD apps


## 📜 License

This is the public demo of StackZero, shared for learning and preview purposes.  
The full version (including core backend logic) is available via the paid setup service.  
Not intended for redistribution or production use without a license.


## 🤖 Author

Based on work by [Eduards Sizovs](https://sizovs.net). Enhanced & maintained by [Robert Fent](https://robertfent.com).

Feel free to reach out if you are interested in using this setup.
