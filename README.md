## x-ui-pro (x-ui + nginx) modification of https://github.com/GFW4Fun/x-ui-pro for REALITY
- Auto Installation (lightweight)
- Auto SSL renewal / Daily reload Nginx X-ui
- Handle **REALITY** and **WebSocket/GRPC/HttpUgrade/SplitHttp** via **nginx**.
- Multi-user and config via port **443**
- More security and low detection with nginx
- Compatible with Cloudflare (only for WebSocket/GRPC/HttpUgrade/SplitHttp)
- Random 150+ fake template!
- Linux Debian/Ubuntu!
  >
  > **You need TWO domains or subdomains**
  > 1. For panel and WebSocket/GRPC/HttpUgrade/SplitHttp
  > 2. For REALITY destination
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
> panel (0=alireza 1=MHSanaei 2=FranzKafkaYu)
> 

**Uninstall X-UI-PRO**:x:
```
sudo su -c "bash <(wget -qO- https://raw.githubusercontent.com/GFW4Fun/x-ui-pro/master/x-ui-pro.sh) -uninstall yes"
```

➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖
### Server Configuration :wrench:🐧⚙️
![](https://github.com/mozaroc/x-ui-pro/blob/master/media/reality.png?raw=true)

## Enable Subscription :link:
#### XUI Panel > Panel Setting > Subscription > Enable Service (Don't change /sub/ /json/)
#### then scroll down to Reverse Proxy URI  add address https://YOUR_PANEL_DOMAIN/SUBSCRIPTIONS_PORT/sub
#### 
➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖
Test ALL
➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖
## Enable UFW :no_entry_sign: Firewall (Prevent direct access to x-ui-xray ports)
```
apt update && apt install ufw
ufw reset && ufw allow ssh && ufw allow ftp && ufw allow http && ufw allow https
ufw enable && ufw reload && ufw status
```
For vless over websocket configuration reffer https://github.com/GFW4Fun/x-ui-pro/blob/master/README.md
