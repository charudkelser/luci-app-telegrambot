# 🤖 OpenWrt Telegram Bot Controller

[![OpenWrt](https://img.shields.io/badge/OpenWrt-24.10%20%7C%20Supported-blue?style=for-the-badge&logo=openwrt)](https://openwrt.org)
[![Version](https://img.shields.io/badge/Version-1.0.4-brightgreen?style=for-the-badge)](https://github.com/charudkelser/luci-app-telegrambot/releases)
[![License](https://img.shields.io/badge/License-MIT-orange?style=for-the-badge)](LICENSE)

Aplikasi kontrol dan monitoring sistem OpenWrt secara real-time langsung melalui Telegram Bot. Dilengkapi dengan antarmuka LuCI dan fitur auto-start setelah boot.

---

## ⚡ Installation Notes

### OpenWrt <= 24.10

Jalankan perintah berikut via SSH terminal OpenWrt:

```bash
opkg update
wget --no-check-certificate -O /tmp/telebot.ipk [https://github.com/charudkelser/luci-app-telegrambot/raw/main/luci-app-telegrambot_1.0.4_all.ipk](https://github.com/charudkelser/luci-app-telegrambot/raw/main/luci-app-telegrambot_1.0.4_all.ipk)
opkg install /tmp/telebot.ipk
rm /tmp/telebot.ipk


## 🛠️ Features

- **📊 Real-time Monitoring:** Cek status sistem, penggunaan CPU/RAM, dan status jaringan WAN/LAN.
- **⚡ Remote Control:** Eksekusi perintah reboot, restart interface, dan bersihkan cache RAM via Telegram.
- **🛡️ Auto-Start Service:** Bot otomatis berjalan saat STB/Router menyala setelah terhubung ke internet.
- **🌐 LuCI Integration:** Pengaturan Telegram Bot Token & Chat ID dengan mudah melalui Web Interface LuCI.

---

## ⚙️ Configuration

1. Buka LuCI Web Interface router Anda.
2. Masuk ke menu **Services** -> **Telegram Bot**.
3. Masukkan **Bot Token** (dari `@BotFather`) dan **Chat ID** Anda.
4. Centang **Enable** lalu klik **Save & Apply**.
