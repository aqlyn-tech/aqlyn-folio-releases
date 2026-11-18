# Aqlyn Folio releases

Downloads of **Aqlyn Folio**, the browser-based report designer and viewer.

## Install with Docker (Dokploy, Coolify, any Docker host)

```
docker run -d -p 5080:5080 -v aqlyn-data:/app/data ghcr.io/aqlyn-tech/aqlyn-folio:latest
```

Use a fixed version such as `ghcr.io/aqlyn-tech/aqlyn-folio:1.0.0` in production. Everything Aqlyn
Folio keeps (reports, users, connections) is in `/app/data`, so keep that volume.

## Install on Windows, Linux or macOS without Docker

1. Install [Node.js](https://nodejs.org) 20.12 or newer.
2. Download `aqlyn-folio-<version>.zip` from the [latest release](../../releases/latest) and unpack it.
3. In the unpacked folder, run `node packages/server/dist/main.js` and open http://localhost:5080.

Optional settings go in a `.env` file next to `package.json`; `.env.example` lists them.

## Licence

The 14-day trial starts on first run. To keep using Aqlyn Folio, buy a licence and enter the key
under **Help › Licence**.
