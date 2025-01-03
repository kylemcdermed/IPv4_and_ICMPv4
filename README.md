# TUN/TAP Device Handler

This project provides an implementation for allocating and working with TUN/TAP virtual network devices. The code demonstrates how to set up and manage a TUN/TAP device, read frames from the device, and handle Ethernet frames.

## Features

- Cross-platform compatibility: The code includes conditional compilation for Linux and Windows systems.
- Implementation of basic networking headers:
  - Ethernet Header
  - ARP Header and IPv4 Payload
  - IPv4 Header
  - ICMP Header (including Echo and Destination Unreachable)
- Mock implementations for reading and handling Ethernet frames.
- Example of calculating Internet checksum.

## Prerequisites

### Linux
- A system with `/dev/net/tun` support is required.
- Root privileges may be necessary to allocate TUN/TAP devices.

### Windows
- TUN/TAP allocation is not supported in the current implementation.
- The program will display an error if run on Windows.
