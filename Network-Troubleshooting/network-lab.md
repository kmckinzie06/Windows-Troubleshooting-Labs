# Network Connectivity Investigation

## Objective

Practice using built-in Windows command-line tools to examine network configuration, test connectivity, and verify DNS resolution.

## Environment

- Operating System: Windows 11
- Tools: Command Prompt, ipconfig, ping, nslookup
- Network adapters: Ethernet and VMware virtual adapters

## Investigation

### 1. Network Configuration

Command used:

`ipconfig`

Findings:

- IPv4 address: Private address assigned by DHCP
- Subnet mask: `255.255.255.0`
- Default gateway: Local network router
- Multiple IPv6 addresses were assigned.
- Two VMware virtual network adapters were also present.

### 2. Local Gateway Connectivity

Command used:

`ping [Default Gateway]`

Result: Successful. The default gateway responded to all four requests.

### 3. External IPv4 Connectivity

Command used:

`ping 8.8.8.8`

Result: Successful. All four packets were received with no packet loss.

Average response time: 18 ms.

### 4. Domain Connectivity and DNS

Commands used:

`ping google.com`

`nslookup google.com`

Results:

- Google.com successfully resolved to IPv4 and IPv6 addresses.
- Ping requests to Google's IPv6 address succeeded.
- DNS queries returned multiple IP addresses.
- No packet loss occurred during the ping test.

## Conclusion

The investigation confirmed that the computer had working local network connectivity, external IPv4 connectivity, IPv6 connectivity, and DNS resolution.

No network connectivity problems were identified during testing.

## Skills Practiced

- Examining network configuration with ipconfig
- Identifying IP addresses, subnet masks, and default gateways
- Testing local and external connectivity with ping
- Understanding IPv4 and IPv6
- Investigating DNS resolution with nslookup
