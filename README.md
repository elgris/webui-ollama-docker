# webui-ollama-docker

Just a Docker Compose file to launch WebUI and Ollama containers. Focused on ROCm support, because I'm running this on a laptop with AMD RX 6700S GPU (Asus G14).

## How to use

```bash
docker compose up
```

The command will start 2 containers:
- WebUI: binds to `localhost:3000`, stores data at `$HOME/.open-webui`, has auth disabled by default.
- Ollama: binds to `localhost:11434`, stores data at `$HOME/.ollama`.

You can also just run `docker compose up ollama` if you need Ollama only.
