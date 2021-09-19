# Enable SSL for your domain

This demo will use the Nginx Ingress Controller, so be sure to have it installed before proceeding.

Further this will only work for non-wildcard domains because we'll use the `HTTP Validation Challenge` and not the `DNS Validation` one.

1. Install [Certificate Manager](https://cert-manager.io/docs/installation/)

2. Grab your public IP address: `kubectl -n ingress-nginx get svc`

3. Add your IP and your E-Mail to the appropriate parts of the .yaml files.