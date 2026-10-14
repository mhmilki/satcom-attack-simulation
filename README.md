# Satellite Communication Attack Simulation — Setup Log

**Project:** Simulating and Detecting Cyber Attacks on Satellite Communication Links: 
A SPARTA and MITRE ATT&CK-Based Approach

**Student:** Mahfujul Islam (25032584)  
**Module:** LD7028 — MSc Cyber Security, Northumbria University

## Overview
This repository tracks the setup, configuration, and progress of a satellite 
simulation testbed using **NOS3** (NASA Operational Simulator for Small Satellites), 
used to replicate and detect cyber attacks on satellite communication links.

## Environment
- **Primary machine:** Microsoft Surface Laptop (16GB RAM, Core i7)
- **Storage:** External HDD (used for NOS3 files due to limited C: drive space)
- **Virtualisation:** Vagrant + VirtualBox
- **Framework:** NOS3 (NASA open-source satellite simulation framework)

## Setup Progress

### 1. Vagrant Installation
- Initially downloaded the wrong Vagrant installer
- Corrected and installed the proper version for Windows

### 2. NOS3 Download
- Cloned the NOS3 repository via Git
- Redirected the download/storage location to the external HDD to avoid 
  filling the C: drive

### 3. Shared Folder / Guest Additions Issue
- After running `make prep`, the project directory inside the VM appeared empty
- Root cause: shared folder between host and VM was not mounting correctly 
  (Guest Additions issue)
- Fix in progress: restarting VM with `vagrant up` to force proper shared 
  folder mount

## Screenshots
See `/screenshots` for visual record of each setup stage.

## Next Steps
- [ ] Confirm shared folder mounts correctly after `vagrant up`
- [ ] Verify NOS3 source files are visible inside VM
- [ ] Begin simulating target attack scenarios
- [ ] Map simulated attacks to SPARTA and MITRE ATT&CK frameworks
- [ ] Develop detection scripts
