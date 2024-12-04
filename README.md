## x-ui-pro (x-ui + nginx) modification of https://github.com/GFW4Fun/x-ui-pro for REALITY
- Auto Installation (lightweight)
- Auto SSL renewal / Daily reload Nginx X-ui
- Handle **REALITY** and **WebSocket** via **nginx**.
- Multi-user and config via port **443**
- Auto enabled subscriptions via port **443**
- Auto configured VLESS+Reality and VLESSoverWebSocket
- Auto configured Firewall
- More security and low detection with nginx
- Compatible with Cloudflare (only for WebSocket/GRPC)
- Random 150+ fake template!
- Linux Debian12/Ubuntu24!
  >
   **You need TWO domains or subdomains**
  1. For panel and WebSocket/GRPC/HttpUgrade/SplitHttp
  2. For REALITY destination
  >
  Get Free subdomains - https://scarce-hole-1e2.notion.site/14d1666462e48069818cf42553bfae1f?pvs=74
  >
  RU instruction - https://scarce-hole-1e2.notion.site/3X-UI-pro-with-REALITY-panel-and-inbaunds-on-port-443-10d1666462e48085be0fee4c136ce417
  
➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖

**Install X-UI-PRO**

```
sudo su -c "bash <(wget -qO- https://github.com/mozaroc/x-ui-pro/raw/refs/heads/master/x-ui-pro.sh) -install yes -panel 1 -ONLY_CF_IP_ALLOW no"
```
> 
> Do not change SubDomain for renew SSL❗
> ##
> panel (0=alireza 1=MHSanaei)
> 

**Uninstall X-UI-PRO**:x:
```
sudo su -c "bash <(wget -qO- https://raw.githubusercontent.com/GFW4Fun/x-ui-pro/master/x-ui-pro.sh) -uninstall yes"
```

➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖
### Server Configuration :wrench:🐧⚙️
>
Reality example
>
![](https://github.com/mozaroc/x-ui-pro/blob/master/media/new_screen_old.png?raw=true)
>
WebSocket example
>
![](https://github.com/mozaroc/x-ui-pro/blob/master/media/vlessandws.png?raw=true)
