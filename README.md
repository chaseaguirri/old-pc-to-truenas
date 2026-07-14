# Turning an Old Family Computer into a Working Network Attached Storage (NAS) Server

> Repurposing outdated hardware into a fully functional TrueNAS server while documenting the entire build process, troubleshooting, testing, and lessons learned.

<!-- <img width="3024" height="4032" alt="IMG_5123" src="https://github.com/user-attachments/assets/f5071f7e-4553-46a4-9a4d-7187356951e8" /> -->

---

# Overview

This repository documents my process of turning an old family desktop computer that had been collecting dust in a closet into a fully functional Network Attached Storage (NAS) server using TrueNAS Community Edition.

Rather than purchasing dedicated hardware, I challenged myself to use as much equipment as I could already find around my house. The result was a functioning NAS capable of storing and sharing files across my home network using enterprise-inspired technologies such as ZFS storage pools, SMB file sharing, user management, and storage quotas.

The goal of this project wasn't simply to install TrueNAS—it was to understand **how** a NAS works, troubleshoot the inevitable problems along the way, and document the entire experience from beginning to end.

---

# Project Goals

* Repurpose unused hardware into something useful.
* Learn the fundamentals of TrueNAS.
* Gain hands-on experience with storage management and networking.
* Configure users, permissions, and shared storage.
* Validate the system through real-world testing.
* Document everything so the project can be reproduced.

---

# Supplies and Resources Used

## Hardware

* Old family desktop computer
* 2 TB hard drive
* USB flash drive (TrueNAS boot device)
* Ethernet cable
* HDMI cable
* TV used as a temporary monitor
* Keyboard
* Mouse
* Screwdriver

## Software & Resources

* TrueNAS Community Edition
* TrueNAS Documentation
* Reddit forums
* YouTube
* AI assistance
* Lots of patience

---

# Challenges

Every project has problems. These were mine.

* Initial no-display issue during first boot.
* Cleaning years of dust out of the computer without damaging components.
* Learning the TrueNAS ecosystem from scratch.
* Installing an operating system that expects dedicated storage devices while working with limited hardware.
* Configuring SMB shares and user permissions.
* Understanding ZFS pools, datasets, and quotas.
* First experience configuring and managing services over a local network.
* Convincing my little brother that I *did* need to borrow half of his desk setup.

---

# Testing

Once the NAS was configured, I performed several validation tests to verify that it functioned as expected.

## Functionality

* Successfully created a ZFS storage pool.
* Configured datasets.
* Created SMB network shares.
* Added user accounts.
* Configured storage quotas.
* Uploaded and downloaded files from a Windows client.
* Verified user authentication and permissions.

## Reliability

* Successfully rebooted without configuration loss.
* Verified automatic pool import after reboot.
* Confirmed shared files remained intact.
* Left the server running overnight to verify stability.
* Tested large file transfers across the network.
* Verified recovery after reconnecting the Ethernet cable.

---

# What I Learned

This project introduced me to a much broader range of IT concepts than I originally expected.

Some of the biggest topics I learned included:

* BIOS configuration
* Bootable installation media
* Linux command-line basics
* TrueNAS administration
* ZFS storage management
* SMB networking
* User permissions
* Storage quotas
* Network troubleshooting
* System validation
* Technical documentation

The biggest takeaway was realizing that building a server is much less about following instructions and much more about troubleshooting unexpected problems until everything finally works.

---

# Hardware

| Component   | Specification                  |
| ----------- | ------------------------------ |
| CPU         | Intel Core i5 (4th Generation) |
| Memory      | 8 GB DDR3                      |
| Storage     | 2 TB HDD                       |
| Boot Device | USB Flash Drive                |
| Network     | Gigabit Ethernet               |
| Platform    | ASUS Desktop                   |

*(The system dates back to roughly 2009 based on BIOS information and had been unused for several years before this project.)*

---

# Final Thoughts

This project accomplished exactly what I wanted it to.

The objective was never to permanently own a NAS—it was to learn how one is built, configured, tested, and maintained using real hardware. After completing testing and documenting the build, the machine was retired and will eventually be repurposed into future Linux server projects.

For a computer that was headed toward becoming e-waste, I'd call that a pretty successful second life.

---

*"One person's tech trash became my first homelab server."*
