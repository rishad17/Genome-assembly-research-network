# Servers

Server configuration exported from the Packet Tracer file (static IPs, services, DHCP pools, DNS records).


## SLC-DNS

- IP: `59.98.0.2` / `255.255.252.0`, gateway `59.98.0.1`
- Services enabled: DNS, HTTP

| DNS name | Type | Address |
|---|---|---|
| mail.motif.bio | A | 59.98.7.2 |
| mail.sequence.bio | A | 59.98.0.4 |
| www.genome-lab.bio | A | 59.98.0.3 |

## SLC-WEB

- IP: `59.98.0.3` / `255.255.252.0`, gateway `59.98.0.1`
- Services enabled: HTTP

## SLC-Email

- IP: `59.98.0.4` / `255.255.252.0`, gateway `59.98.0.1`
- Services enabled: HTTP

## SLC-DHCP

- IP: `59.98.0.5` / `255.255.252.0`, gateway `59.98.0.1`
- Services enabled: DHCP, HTTP

| Pool | Network | Mask | Gateway | Range | DNS |
|---|---|---|---|---|---|
| GVU-POOL | 59.98.0.0 | 255.255.255.128 | 59.98.0.1 | 59.98.0.10 – 59.98.0.109 | 59.98.0.2 |
| serverPool | 59.98.8.0 | 255.255.255.128 | 59.98.8.1 | 59.98.8.10 – 59.98.8.109 | 59.98.0.2 |

## MDU-Email

- IP: `59.98.7.2` / `255.255.255.0`, gateway `59.98.7.1`
- Services enabled: HTTP

## MDU-DHCP

- IP: `59.98.7.3` / `255.255.255.0`, gateway `59.98.7.1`
- Services enabled: DHCP, HTTP

| Pool | Network | Mask | Gateway | Range | DNS |
|---|---|---|---|---|---|
| serverPool | 59.98.7.0 | 255.255.255.0 | 59.98.7.1 | 59.98.7.10 – 59.98.7.255 | 59.98.0.2 |
