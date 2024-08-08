

```markdown
# Mini-VPN Implementation

## Overview

This repository contains a Python-based implementation of a basic Virtual Private Network (VPN) using TUN/TAP interfaces and UDP for communication. The VPN facilitates secure and efficient data transfer between two endpoints.

## Features

- **TUN/TAP Interface Creation**: Establishes virtual network devices on both client and server sides.
- **UDP Communication**: Manages packet forwarding between the TUN interface and UDP sockets.
- **Packet Handling**: Uses `scapy` for network packet manipulation.

## Files

### `client.py`
Sets up a TUN interface on the client side, assigns an IP address, and handles packet forwarding to/from a UDP socket.

### `server.py`
Sets up a TUN interface on the server side, assigns an IP address, and manages UDP communication with the client.

## Requirements

- Python 3.x
- `scapy` library

Install the required Python library using:

```bash
pip install scapy
```

## Usage

1. **Run the Server:**

   ```bash
   sudo python3 server.py
   ```

2. **Run the Client:**

   ```bash
   sudo python3 client.py
   ```

   Ensure you configure the `ip` and `port` variables in both scripts to match your server and client settings.

## Notes

- Requires superuser privileges to create and manage TUN/TAP interfaces.
- Ensure proper permissions are granted for network interface management.

## Contributing

Feel free to submit issues or pull requests for improvements or bug fixes.

## Contact

For questions or feedback, reach out to:

- Email: vimenon@syr.edu
- LinkedIn: [Vinay Menon](https://linkedin.com/in/vinay-menon-1b3055219/)



This `README.md` file provides a clear and concise description of your project, how to use it, and how to reach out for further communication.
