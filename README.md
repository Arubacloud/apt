# Arubacloud apt repository

Official apt repository for the [Aruba Cloud CLI](https://github.com/Arubacloud/acloud-cli).

## Install

```bash
curl -fsSL https://arubacloud.github.io/apt/gpg.key | sudo gpg --dearmor -o /etc/apt/keyrings/arubacloud.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/arubacloud.gpg] https://arubacloud.github.io/apt stable main" | sudo tee /etc/apt/sources.list.d/arubacloud.list
sudo apt update
sudo apt install acloud
```
