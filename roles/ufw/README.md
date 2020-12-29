# UFW

## Overview

Disables all incoming and outgoing connections, with the following exceptions:

- Allows all incoming SSH connections from the list of IPs in the `allowed_ips` variable. This connection is rate limited.
- Allows all incoming and outgoing NTP connections.

Logging is enabled at the default level.

## Variables

- `allowed_ips`: The path on the local machine to the public key which will be used to access the server. Defaults to:

    ```yaml
  - "192.168.0.15"
  - "192.168.0.13"
    ```
