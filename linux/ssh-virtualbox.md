SSH ilə VirtualBox VM-ə qoşulma

Addım 1 — NAT Port Forwarding
Settings → Network → Adapter 1 (NAT) → Advanced → Port Forwarding
- Host Port: 2222
- Guest Port: 22


Addım 2 — VM içində SSH server qur
sudo apt update && sudo apt install -y openssh-server
sudo systemctl enable ssh


Addım 3 — Host maşından qoş
ssh -p 2222 istifadeci_adi@127.0.0.1
