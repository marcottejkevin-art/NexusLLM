# Nexus Homelab — Network Security

AI server: `192.168.1.114`

Mini PC: `192.168.1.112`

Tailscale: `100.117.255.81`

UFW:
- default incoming deny
- default outgoing allow
- default routed deny
- allow `192.168.1.0/24`
- allow `tailscale0`

Portainer Agent:
- TCP/9001
- source allowed: `192.168.1.112`
- restricted by Docker `DOCKER-USER`
- persistent service: `portainer-firewall.service`

Do not store credentials or webhook secrets in the Knowledge Base.
