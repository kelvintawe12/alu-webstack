# Webstack Configuration Project

This repository contains the files and configurations for setting up a web infrastructure using HAproxy for load balancing, SSL termination, and enforcing HTTPS on a web stack running on **Ubuntu 16.04 LTS**. The project covers tasks related to DNS configuration, SSL certificate management, and HTTP to HTTPS redirection.

---

## Project Structure

The project consists of the following files:
---

## Overview

### Tasks to Complete:
1. **Configure DNS Records**:
   - Set up multiple subdomains and point them to the corresponding server IPs for load balancing.
   
2. **Set Up SSL Termination**:
   - Use HAproxy to handle SSL-encrypted traffic and forward unencrypted traffic to backend web servers.

3. **Force HTTPS**:
   - Configure HAproxy to ensure all traffic uses HTTPS and automatically redirect any HTTP requests.

---

## Requirements

### Allowed Editors:
- You may use the following editors to write scripts and configurations:
  - `vi`
  - `vim`
  - `emacs`

### System Requirements:
- All files and configurations are designed to work on **Ubuntu 16.04 LTS**.

### Bash Script and File Formatting:
- Ensure all files end with a new line.
- **README.md**: A mandatory `README.md` file must be present at the root of your project.
- **Bash Scripts**:
  - The first line of each Bash script should be: `#!/usr/bin/env bash`.
  - The second line should contain a comment explaining the script's purpose.
  - Bash scripts must pass **Shellcheck** (version 0.3.7) without any errors.
  - Use `awk` and at least one Bash function in your scripts.

---

## Tasks

### 0. **World Wide Web**
#### Goal:
- Configure DNS records for the subdomains `www`, `lb-01`, `web-01`, and `web-02`.
- Write a Bash script (`0-world_wide_web`) that accepts a domain name and optional subdomain to display the DNS information.

#### Requirements:
1. Add `www`, `lb-01`, `web-01`, and `web-02` subdomains to your domain, pointing to the respective server IPs.
2. The script should accept two arguments:
   - `domain`: The domain to audit.
   - `subdomain` (optional): The specific subdomain to audit.
3. The output should display in this format:


## Installation and Setup

### Prerequisites:
1. **Ubuntu 16.04 LTS**: The setup is designed for Ubuntu 16.04 LTS.
2. **HAproxy 1.5+**: Ensure you have HAproxy version 1.5 or higher installed.
3. **Certbot**: Used for obtaining SSL certificates for your domain.
4. **Shellcheck**: Used for validating Bash scripts (version 0.3.7).
