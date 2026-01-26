## 👋 Welcome to emby 🚀

Media server for organizing and streaming personal media

## 📋 Description

Media server for organizing and streaming personal media

## 🚀 Services

- **emby**: emby/embyserver:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/emby/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/emby" ~/.local/srv/docker/emby
cd ~/.local/srv/docker/emby
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install emby
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
SERVICE_USER=1000
SERVICE_GROUP=1000
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:8096

## 📂 Volumes

- `./rootfs/config/emby` - Data storage
- `./rootfs/data/emby` - Data storage

## 🔍 Logging

```shell
docker compose logs -f emby
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
