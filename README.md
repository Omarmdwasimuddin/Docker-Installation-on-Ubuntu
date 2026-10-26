## Docker Installation on Ubuntu

#### Update System Packages
```bash
sudo apt-get update
```
---

#### Install Required Dependencies
```bash
sudo apt-get install -y ca-certificates curl gnupg
```
---

#### Add Docker’s Official GPG Key
```bash
sudo install -m 0755 -d /etc/apt/keyrings
```
```bash
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | \
sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
```
```bash
sudo chmod a+r /etc/apt/keyrings/docker.gpg
```
---

####
```bash

```
---

####
```bash

```
---
