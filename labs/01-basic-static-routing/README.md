# Lab 01: Basic Two-LAN Static Routing

## Objective

Build two separate LANs connected by two routers and configure static routing so that devices on both networks can communicate.

## Topology

![Network topology](topology.png)

## Devices

- 2 routers: R1 and R2
- 2 switches: S1 and S2
- 2 PCs: PC1 and PC2

## Addressing plan

| Device  | IP address |
|---|---|---|
| PC1 | 192.168.10.10/24 |
| R1 | 192.168.10.1/24 |
| R1 | 10.0.0.1/30 |
| R2 | 10.0.0.2/30 |
| R2 | 192.168.20.1/24 |
| PC2 | 192.168.20.10/24 |

## Configuration tasks

- Configured router interfaces with IP addresses.
- Configured PC IP addresses and default gateways.
- Added static routes on R1 and R2.
- Tested end-to-end connectivity using ping.

## Verification

- [ ] PC1 can ping its default gateway.
- [ ] PC2 can ping its default gateway.
- [ ] PC1 can ping PC2.
- [ ] R1 and R2 routing tables contain the remote-network route.

## What I learned

- Routers connect different IP networks.
- PCs need a correct default gateway to reach remote networks.
- Static routes tell routers where to send traffic for remote networks.
- Ping and routing-table checks help identify connectivity problems.

## Files

- `01-basic-static-routing.pkt` — Cisco Packet Tracer project
- `topology.png` — topology screenshot
