# IIS installation lab

Evidence supplied October 26, 2026. Server: DC01.corp.adtraining.com, 192.168.60.10.

- Screenshot 01 shows IIS Manager with DC01 > Sites > Default Web Site selected. Start is disabled and Stop is available, indicating the site is running. Browse *:80 (http) is available.
- Screenshot 02 shows the default IIS welcome page loaded at localhost inside DC01, verifying local HTTP content delivery.

An installation-success wizard screenshot was not supplied. Access from another computer, firewall traversal, custom content, host-name bindings, and HTTPS have not been tested.

During setup, Server Manager showed red Manageability tiles with Online - Restart pending. The user restarted Windows Server; roles finished loading and the user confirmed the red alerts cleared.
