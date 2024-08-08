# Mini-VPN Implementation

## Overview

This project demonstrates a basic Virtual Private Network (VPN) implementation using Python. It involves the creation and management of TUN/TAP network interfaces, as well as the handling of UDP communication for data transfer. The solution includes both client and server components for establishing a VPN connection.

## Features

- **TUN/TAP Interface**: Configures virtual network interfaces for packet forwarding.
- **UDP Packet Forwarding**: Implements UDP sockets to relay packets between the TUN interface and the network.
- **Packet Processing**: Utilizes `scapy` for packet manipulation and analysis.

## Components

### `client.py`

- Initializes a TUN interface and assigns an IP address.
- Forwards packets between the TUN interface and a UDP socket to a specified server address.

### `server.py`

- Sets up a TUN interface and assigns an IP address.
- Receives packets via UDP and forwards them through the TUN interface to the client.

## Requirements

- Python 3.x
- `scapy` library

Install the necessary Python library using:

```bash
pip install scapy


sudo python3 server.py

sudo python3 client.py
