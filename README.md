# ReadMe
This acts a self/Azure hosted substitute for Uptime Robot, as they are changing their pricing plan.
![Current status (will not show when doen of course)](https://uptime.robertsirre.nl/api/badge/9/status) ![](https://uptime.robertsirre.nl/api/badge/9/uptime/48)

## How to deploy
*Google as this may change.*
I registered an Azure context, and performed a simple `docker compose up -d`, this may become obsolete.

## SSL
See [Azure docs > Enable automatic HTTPS with Caddy in a sidecar container](https://learn.microsoft.com/en-us/azure/container-instances/container-instances-container-group-automatic-ssl)
Also see: [GitHub > uptime-kuma > Reverse Proxy](https://github.com/louislam/uptime-kuma/wiki/Reverse-Proxy) (Cloudflare Tunnels may have been simpler)

> Note: `Caddyfile` needs to be added manually to Azure share `proxy-caddyfile`