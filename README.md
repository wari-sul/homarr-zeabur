---

# Homarr Zeabur Template

A fully optimized **one-click deployment template** for **[Homarr](https://homarr.dev)** — the modern, elegant dashboard for organizing and managing your self-hosted apps and services.

[![Deploy on Zeabur](https://zeabur.com/button.svg)](https://zeabur.com/templates/F9YBW5)

This repository contains the **latest maintained version** of the Homarr Zeabur template.

---

## 🚀 Features

* 🖥️ **Clean, modern, customizable interface**
* 📱 **Responsive and mobile-friendly**
* 💾 **Persistent data storage** via Zeabur volumes (`/appdata`)
* 🔐 **Secure secret encryption** using your custom key
* 🌐 **Automatic HTTPS + domain setup** through Zeabur
* 🧩 **Compatible with the official Homarr Docker image**

---

## ⚡ Quick Deploy

1. Click the **Deploy on Zeabur** button
   👉 [https://zeabur.com/templates/F9YBW5](https://zeabur.com/templates/F9YBW5)
2. Configure the required environment variables:

   * **Dashboard Domain** – custom or Zeabur-provided domain
   * **SECRET_ENCRYPTION_KEY** – generate with:

     ```bash
     openssl rand -hex 32
     ```
   * **TZ** (optional) – e.g., `America/New_York`, `Asia/Tokyo`
3. Deploy and access your dashboard at the generated URL.

---

## 🔧 Configuration Details

All persistent data is stored under:

```
/appdata
```

Includes:

* Dashboard layout
* App configurations
* Icons & metadata
* User preferences

### Environment Variables

| Variable                | Required   | Description                                 |
| ----------------------- | ---------- | ------------------------------------------- |
| `SECRET_ENCRYPTION_KEY` | ✅ Yes      | 64-character hex key for encrypting secrets |
| `TZ`                    | ❌ Optional | Container timezone (e.g., `Europe/London`)  |

---

## 📦 Manual Deployment

If deploying directly from this repository:

```bash
zeabur template deploy -f homarr-template.yaml
```

---

## 🔗 Useful Links

* **Published Template:** [https://zeabur.com/templates/F9YBW5](https://zeabur.com/templates/F9YBW5)
* **Homarr Documentation:** [https://homarr.dev/docs](https://homarr.dev/docs)
* **Docker Image:** [https://github.com/homarr-labs/homarr/pkgs/container/homarr](https://github.com/homarr-labs/homarr/pkgs/container/homarr)

---

## 📜 License

MIT License

---
