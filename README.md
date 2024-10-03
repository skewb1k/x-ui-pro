## x-ui-pro (x-ui + warp + nginx) modification of https://github.com/GFW4Fun/x-ui-pro for REALITY
- Auto Installation (lightweight)
- Auto SSL renewal / Daily reload Nginx X-ui
- Handle **REALITY** and **WebSocket/GRPC/HttpUgrade/SplitHttp** via **nginx**.
- Multi-user and config via port **443**
- More security and low detection with nginx
- Compatible with Cloudflare (only for WebSocket/GRPC/HttpUgrade/SplitHttp)
- Random 150+ fake template!
- Linux Debian/Ubuntu!
  >
  > **You need TWO domains or subdomain**
  > 1. For panel and WebSocket/GRPC/HttpUgrade/SplitHttp
  > 2. For REALITY destination
  >   
  
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
![](https://raw.githubusercontent.com/GFW4Fun/x-ui-pro/master/media/Config_XUI_ADMIN_4.jpg)
![](https://raw.githubusercontent.com/GFW4Fun/x-ui-pro/master/media/grpc_config_format.jpg)
➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖
### Client Configuration :white_check_mark:	:computer:🔌
![](https://raw.githubusercontent.com/GFW4Fun/x-ui-pro/master/media/XUI_CONFIG_XRAY_CLIENT_EDIT2.png)
➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖
### Enable WARP<img src="https://raw.githubusercontent.com/GFW4Fun/x-ui-pro/master/media/cdnon.png" width="34"> (Fix Error 403-Forbidden Google Search)
![](https://raw.githubusercontent.com/GFW4Fun/x-ui-pro/master/media/error403Google.png)
#### XUI PANEL> Xray Configs> Outbands > Add WARP > Create > Add > Save Restart!
![](https://raw.githubusercontent.com/GFW4Fun/x-ui-pro/master/media/Enable_WARP.jpg)
#### XUI PANEL> Xray Configs> Routing Rules> Add Rules > 
#### Inbound Tags (Select Your Configs/inbounds) + Outbound Tag (WARP outbound) > Add rule! > Save Restart!
➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖
## Enable Subscription :link:
#### XUI Panel > Panel Setting > Subscription > Enable Service (Don't change /sub/ /json/)
#### XUI Panel > Inbounds > General Actions > Export All URLs - Subscriptions
#### In the displayed address, change `  :  to  /  `
➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖
## Enable UFW :no_entry_sign: Firewall (Prevent direct access to x-ui-xray ports)
```
apt update && apt install ufw
ufw reset && ufw allow ssh && ufw allow ftp && ufw allow http && ufw allow https
ufw enable && ufw reload && ufw status
```
➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖➖
## Cloudflare Find Good IP (VPN off❗ during scanning)
Cloudflare IP Ranges: https://www.cloudflare.com/ips/

Cloudflare IP Scanner: [vfarid](https://vfarid.github.io/cf-ip-scanner/) | [goldsrc](https://cloudflare-scanner.vercel.app) | [ircfspace](https://ircfspace.github.io/scanner/) | [drunkleen](https://drunkleen.github.io/ip-scanner/) | [cloudflare-v2ray-scanner](https://cloudflare-v2ray.vercel.app/)
##
### Please Star ⭐ Thank you!

