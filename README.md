
---

# Homarr Zeabur Template

A fully optimized **one-click deployment template** for **[Homarr](https://homarr.dev)** — the modern, elegant dashboard for organizing and managing your self-hosted apps and services.

[![Deploy on Zeabur](https://zeabur.com/button.svg)](https://zeabur.com/templates/C2O8R8)

This repository contains the **latest maintained version** of the Homarr Zeabur template.

---

## 🚀 Features

* 🖥️ **Clean, modern, customizable interface**
* 📱 **Responsive and mobile-friendly UI**
* 💾 **Persistent data storage** via Zeabur volumes (`/appdata`)
* 🔐 **Secure secret storage** (required encryption key)
* 🌐 **Automatic HTTPS + domain management** through Zeabur
* 🧩 **Fully compatible with the official Homarr Docker image**

---

## ⚡ Quick Deploy

1. Click the **Deploy on Zeabur** button
   👉 [https://zeabur.com/templates/C2O8R8](https://zeabur.com/templates/C2O8R8)
2. Set the required environment variables:

   * **Dashboard Domain** – your custom domain or Zeabur-provided subdomain
   * **SECRET_ENCRYPTION_KEY** – generate with:

     ```bash
     openssl rand -hex 32
     ```
   * **TZ** *(optional)* – e.g. `America/New_York`, `Asia/Tokyo`
3. Deploy and access your dashboard at the generated URL.

---

## 🔧 Configuration Details

All persistent data is stored under:

```
/appdata
```

This includes:

* Dashboard layout
* App & widget configuration
* Icons, metadata, and preferences

### Environment Variables

| Variable                | Required   | Description                                            |
| ----------------------- | ---------- | ------------------------------------------------------ |
| `SECRET_ENCRYPTION_KEY` | ✅ Yes      | 64-character hex string used to encrypt stored secrets |
| `TZ`                    | ❌ Optional | Container timezone (e.g., `Europe/London`)             |

---

## 📦 Manual Deployment

If you'd like to deploy the template directly from this repository:

```bash
zeabur template deploy -f homarr-template.yaml
```

---

## 🔗 Useful Links

* **Published Template:** [https://zeabur.com/templates/C2O8R8](https://zeabur.com/templates/C2O8R8)
* **Homarr Documentation:** [https://homarr.dev/docs](https://homarr.dev/docs)
* **Docker Image:** [https://github.com/homarr-labs/homarr/pkgs/container/homarr](https://github.com/homarr-labs/homarr/pkgs/container/homarr)

---

## 📜 License

MIT License

---
