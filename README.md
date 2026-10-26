## Docker Installation on Ubuntu

#### Windows e Ubuntu Linux use korar jonno install koro
```bash
wsl --install
```
---

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

#### Set Up Docker Repository
```bash
echo \
"deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
$(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
---

#### Install Docker Engine
```bash
sudo apt-get update
```
```bash
sudo apt-get install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
---

#### Verify Docker Installation
```bash
sudo docker run hello-world
```
---
