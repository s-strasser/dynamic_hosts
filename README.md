## Installation
1. Download this repository using git or http.
2. Navigate to the folder with the files using a terminal.
3. Make sure you have got root permissions (e.g. you're logged in as root or you use sudo)
4. Execute the following command: ./dynamic-hosts-setup
5. Configure your hosts at /etc/dynamic_hosts/hosts

## Configuration: /etc/dynamic_hosts/hosts
Every line stands for one host-entry:

    myDevServer.local: officeDevServer.dyndns.example.com 
    
Also you can define multiple targets. Using this feature you can for example use the internal connection (e.g. 10.10.10.1) while your at office and switch to the dyndns-based external connection when you're at home.

    myDevServer.local: officeDevServer.local officeDevServer.dyndns.example.com

Until now there are no comments possible. This is planed in a future release.

## Feature list
- Resolves /etc/hosts - entries dynamically based on dns
- Updates entries every 5 minutes
- Can resolve multiple targets and choose the first on available with the highest priority

## Changelog
### v 1.0
- Initial release 
