# Unraid Templates
- [Sure-Web](#sure-web)
  * [Additional Requirements](#additional-requirements)
  * [First installation](#first-installation)
- [Sure-Worker](#sure-worker)
  * [Additional Requirements](#additional-requirements)
  * [First installation](#first-installation)

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
![Sure-Web](https://raw.githubusercontent.com/Skylinar/unraid_templates/refs/heads/main/images/readme/sure-worker-128.png)

Coming soon...

**[`^back to top^`](#unraid-templates)**

----