# Unraid Templates
- [Home-Hub](#home-hub)
  * [First installation](#first-installation)
- [Pi-Dash](#pi-dash)
  * [First installation](#first-installation)
- [Repocket](#repocket)
  * [First installation](#first-installation)
- [Sure-Web](#sure-web)
  * [Additional Requirements](#additional-requirements)
  * [First installation](#first-installation)
- [Sure-Worker](#sure-worker)
  * [Additional Requirements](#additional-requirements)
  * [First installation](#first-installation)
- [Traffmonetizer](#traffmonetizer)

----
# Home-Hub
![Home-Hub](https://raw.githubusercontent.com/Skylinar/unraid_templates/refs/heads/main/images/homehub.png)

Ever wanted a simple, private spot on your home network for your family's daily stuff? That's HomeHub. It's a lightweight, self-hosted web app that turns any computer (even a Raspberry Pi!) into a central hub for shared notes, shopping lists, chores, a media downloader, and even a family expense tracker.

It's designed to be easy to use for everyone in the family, with a clean interface that works great on any device.

**Application Name:** Home-Hub

**Application Site:** https://github.com/surajverma/homehub

**Registry:** https://github.com/surajverma/homehub/pkgs/container/homehub

**Github:** https://github.com/surajverma/homehub

## First installation 
Before first startup:
1. create the appdata folder:
```
mkdir /mnt/user/appdata/homehub
```
2. grab the example configuration yml:
```
curl https://raw.githubusercontent.com/surajverma/homehub/main/config-example.yml -o /mnt/user/appdata/homehub/config.yml
```
3. adjust the config as needed

**[`^back to top^`](#unraid-templates)**

----
# Pi-Dash
![Pi-Dash](https://raw.githubusercontent.com/Skylinar/unraid_templates/refs/heads/main/images/readme/pi-dash-128.png)

Pi-Dash is a simple, lightweight dashboard for monitoring multiple Pi-hole instances. It provides a clean, at-a-glance, responsive view of your Pi-hole statistics.

**Application Name:** Pi-Dash

**Application Site:** https://github.com/surajverma/pi-dash

**Registry:** https://github.com/surajverma/pi-dash/pkgs/container/pi-dash

**Github:** https://github.com/surajverma/pi-dash

## First installation 
Before first startup:
1. create the appdata folder: 
```
mkdir /mnt/user/appdata/pi-dash
```
2. grab the example configuration json: 
```
curl https://raw.githubusercontent.com/surajverma/pi-dash/refs/heads/main/config-example.json -o /mnt/user/appdata/pi-dash/config.json
```
3. adjust the config as needed

**[`^back to top^`](#unraid-templates)**

----

# Repocket
![Repocket](https://raw.githubusercontent.com/Skylinar/unraid_templates/refs/heads/main/images/readme/repocket-128.png)

With Repocket, you can earn passive income by sharing your unused internet bandwidth safely and easily. Start making money today, just set up, connect, and let Repocket work in the background. Sign up using link: https://link.repocket.com/drQ5

## First Installation:
Before starting the container you should replace 'your_token_here' in the Post Args.

**Application Name:** Repocket

**Application Site:** https://link.repocket.com/drQ5

**Registry:** https://hub.docker.com/r/repocket/repocket/

**[`^back to top^`](#unraid-templates)**

----
# Sure-Web
![Sure-Web](https://raw.githubusercontent.com/Skylinar/unraid_templates/refs/heads/main/images/readme/sure-web-128.png)

Sure is a community-driven fork of the former Maybe Finance application, continuing its mission to help users manage personal finances by tracking expenses, budgeting, and supporting wealth management.
Note: "Maybe" is a trademark of Maybe Finance, Inc..

This is the 1 of 2 containers required to run Sure finance; **please review the additional requirements.**

**Application Name:** Sure-Web

**Application Site:** https://github.com/we-promise/sure

**Registry:** https://github.com/we-promise/sure/pkgs/container/sure

**Github:** https://github.com/we-promise/sure
## Additional Requirements
This is container 1 of 2 needed to run Sure finance, runs alongside **Sure-Worker**.
Requires a **Postgres** database and **Redis**.

Check the Sure documentation for more information: https://github.com/we-promise/sure/blob/main/docs/hosting/docker.md
## First installation 
To ensure correct user permissions for the app-storage folder, **run** `chown -R 1000:1000 /mnt/user/appdata/sure/app-storage` after the initial startup.

**[`^back to top^`](#unraid-templates)**

----
# Sure-Worker
![Sure-Worker](https://raw.githubusercontent.com/Skylinar/unraid_templates/refs/heads/main/images/readme/sure-worker-128.png)

Sure is a community-driven fork of the former Maybe Finance application, continuing its mission to help users manage personal finances by tracking expenses, budgeting, and supporting wealth management.
Note: "Maybe" is a trademark of Maybe Finance, Inc..

This is the 2 of 2 container required to run Sure finance; **please review the additional requirements.**

**Application Name:** Sure-Worker

**Application Site:** https://github.com/we-promise/sure

**Registry:** https://github.com/we-promise/sure/pkgs/container/sure

**Github:** https://github.com/we-promise/sure

**[`^back to top^`](#unraid-templates)**

----

# Traffmonetizer
![Traffmonetizer](https://raw.githubusercontent.com/Skylinar/unraid_templates/refs/heads/main/images/readme/traffmonetizer-128.png)

With Traffmonetizer, you can earn passive income by sharing your unused internet bandwidth safely and easily. Start making money today, just set up, connect, and let Traffmonetizer work in the background. Sign up using link: https://traffmonetizer.com/?aff=1674311

**Application Name:** Traffmonetizer

**Application Site:** https://traffmonetizer.com/?aff=1674311

**Registry:** https://hub.docker.com/r/traffmonetizer/cli_v2/

**[`^back to top^`](#unraid-templates)**

----