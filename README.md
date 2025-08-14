# Waste Repo - Installation Guide

Follow these steps to add the Waste Repo to your Debian-based system (e.g., Debian 12 Bookworm).

## 1. Add the repository key

```bash
sudo mkdir -p /etc/apt/keyrings
curl -fsSL https://zs-247.github.io/wasteofarepo/repo.asc | sudo gpg --dearmor -o /etc/apt/keyrings/wasteofarepo.gpg
# add repository
echo "deb [signed-by=/etc/apt/keyrings/wasteofarepo.gpg] https://zs-247.github.io/wasteofarepo bookworm main" | sudo tee /etc/apt/sources.list.d/wasteofarepo.list
```
## Install waste
```bash
sudo apt update
sudo apt install waste
```
