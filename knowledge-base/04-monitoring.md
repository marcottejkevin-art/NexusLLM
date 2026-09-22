# Nexus Homelab — Monitoring

Uptime Kuma:
- Host: `192.168.1.112`
- Port: `3001`
- URL: `http://192.168.1.112:3001`

Monitors:
- Open WebUI: `http://192.168.1.114:3000`
- Ollama: `http://192.168.1.114:11434/api/tags`
- Nexus-Ai: ping `192.168.1.114`

Notifications use a private Discord server and `#alerts`.

Uptime Kuma 2FA is enabled.

Open WebUI troubleshooting:
1. Check Nexus-Ai.
2. Check open-webui.
3. Check health.
4. Check Ollama.
5. Review logs.
6. Check firewall/networking.

Portainer troubleshooting:
1. Check portainer_agent.
2. Verify TCP/9001 from 192.168.1.112.
3. Check DOCKER-USER.
4. Check portainer-firewall.service.
