
## 📦 Installation Menu
```bash
apt update -y && wget -q https://raw.githubusercontent.com/Fitunnel/FiZivpn/main/install.sh -O /usr/local/bin/zivpn-manager && chmod +x /usr/local/bin/zivpn-manager && /usr/local/bin/zivpn-manager
```
## 📦 Update Menu
```bash
wget -q https://raw.githubusercontent.com/Fitunnel/FiZivpn/main/update.sh -O /usr/local/bin/update-manager && chmod +x /usr/local/bin/update-manager && /usr/local/bin/update-manager
```
## 🧼 Uninstall Menu
```bash
wget -q https://raw.githubusercontent.com/Fitunnel/FiZivpn/main/uninstall.sh -O /usr/local/bin/uninstall-zivpn && chmod +x /usr/local/bin/uninstall-zivpn && /usr/local/bin/uninstall-zivpn
```
## 📦 Fix Menu
```bash
chmod +x /usr/local/bin/zivpn-manager
```
## ⚙️ Systemd / Auto Restart

- Service dijalankan dengan:
```bash
systemctl enable zivpn.service
systemctl start zivpn.service
```
- Service akan **restart otomatis** jika mati
- Tunggu **network-online.target** sebelum start service → mencegah error UDP bind  
