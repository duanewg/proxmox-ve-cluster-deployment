<p align="center">
<img src="assets/proxmox-logo.png" alt="Proxmox Logo" />
</p>

# Proxmox VE Cluster Deployment 
Installed and configured Proxmox VE to provide a platform for hosting a NAS (Network Attached Storage), Domain Controller, Document Management System, file sharing, and backups. This setup ensures centralized management, scalability, and efficient resource utilization, enabling the organization to streamline operations and adapt to evolving business requirements seamlessly.

## Environments and Technologies Used

- 3 x Dell PowerEdge R720xd
    - 2 x Intel Xeon E5-2670 v2 2.50GHz 10-Core
    - 9 x 4TB 7.2K SAS 3.5" 6Gbps hard drives
    - 2 x 450GB 15K SAS 3.5" 6Gbps Hard Disk Drive
    - 1 x 120GB SSD SATA 2.5" 6Gbps Solid State Drive
    - 32GB PC3-10600R ECC RAM
    - Dell 099GTM Quad Port 2x 10G RJ45 + 2x 1GB 

## Operating Systems Used

- Proxmox VE 7.1

## High-Level Deployment and Configuration Steps

- Install severs in rack and connect to network
- Install Proxmox VE on each physical server using a bootable USB with the Proxmox installation ISO
    - Configure the location, time zone, timezone, email, root password, host name, and IP address
- Update the system software on each server
- Access the management GUI and configure storage for each server
- Create a new cluster on one of the servers and copy the cluster join information
- Access the management GUI for the remaining servers and join them to the cluster using the copied join information
- Create VMs as required

<h2>Architecture Diagram</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
