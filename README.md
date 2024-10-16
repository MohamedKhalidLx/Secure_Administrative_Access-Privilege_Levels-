# OSPF and Enhanced Security Network Configuration with SSH

## Overview
This project configures a network with three routers connected via OSPF (Open Shortest Path First). The routers are secured with encrypted passwords, SSH access, and Telnet for remote management. Additionally, the configuration implements enhanced password security using the Scrypt hashing algorithm for user authentication.

## Topology
- **Routers**: R1, R2, R3 (Configured with OSPF for routing and secured with SSH and Telnet access)
- **Switches**: S1, S3
- **End-Devices**: PC-A, PC-C
- **Routing Protocol**: OSPFv2 (IPv4)
- **Interfaces**: Configured with both public and private IP addresses.
- **Security Measures**: Encrypted passwords, SSH configuration, and Telnet for remote access.

## Objectives:
- Configure OSPF for dynamic routing between routers.
- Implement secure access using SSH and Telnet.
- Enhance password security with Scrypt hashing and minimum password length policies.
- Use RSA key pairs and enforce SSHv2 for encrypted communication.

## Network Details:

### Addressing Table:
![Addressing Table](https://github.com/user-attachments/assets/d9f2a73f-1c4e-4a62-b543-ca20d710df69)

### VLAN Table:
N/A (This configuration is focused on routing without VLAN segmentation.)

## Configuration Files:
- **Router 1 (R1)**, **Router 2 (R2)**, and **Router 3 (R3)** configurations are available in the `Configuration%20File%20(Privileg%20Level).txt` file.

## Steps to Implement:
1. **Configure OSPF** on all three routers to enable dynamic routing between networks.
2. **Set up password policies** using Scrypt hashing and minimum password lengths for user accounts.
3. **Secure routers with SSH**:
    - Enforce SSHv2 and RSA encryption.
    - Set SSH timeout and authentication retry values.
4. **Configure Telnet** access for remote management.
5. **Secure console and AUX ports** with encrypted passwords.
6. **Test OSPF routing** by verifying routes in each router's routing table.
7. **Test SSH and Telnet access** to ensure secure remote management is functional.

## How to Use:
1. Clone the repository:
   ```bash
   git clone https://github.com/YourUsername/OSPF-Security-Network-Configuration.git
