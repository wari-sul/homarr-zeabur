# Homarr Zeabur Template

One-click deployment template for [Homarr](https://homarr.dev) - a sleek, modern dashboard for managing your self-hosted apps and services.

[![Deploy on Zeabur](https://zeabur.com/button.svg)](https://zeabur.com/templates/C2O8R8)

## Features

- Modern, customizable dashboard interface
- Mobile-friendly responsive design
- Persistent data storage with Docker volumes
- Automatic SSL and domain management via Zeabur

## Quick Deploy

1. Click the [Deploy on Zeabur](https://zeabur.com/templates/C2O8R8) button
2. Configure required variables:
   - **Dashboard Domain**: Your custom domain or use Zeabur's default
   - **Secret Encryption Key**: Generate with `openssl rand -hex 32`
   - **Timezone**: (Optional) e.g., `America/New_York`, `Asia/Tokyo`
3. Access your dashboard at the provided URL

## Configuration

All data persists in `/appdata` including:
- Dashboard configuration
- App settings and icons
- User preferences

### Environment Variables

- `SECRET_ENCRYPTION_KEY` - Required 64-character hex string for encryption
- `TZ` - Optional timezone setting

## Manual Deployment
`zeabur template deploy -f homarr-template.yaml`


## Links

- [Published Template](https://zeabur.com/templates/C2O8R8)
- [Homarr Documentation](https://homarr.dev/docs)
- [Docker Image](https://github.com/homarr-labs/homarr/pkgs/container/homarr)

## License

MIT License

