# OpenWrt Telegram Bot Controller

Tools untuk kontrol dan monitoring router OpenWrt via Telegram.

## Installation Notes

OpenWrt <= 24.10:

```bash
opkg update
wget --no-check-certificate -O /tmp/telebot.ipk [https://github.com/charudkelser/luci-app-telegrambot/raw/main/luci-app-telegrambot_1.0.4_all.ipk](https://github.com/charudkelser/luci-app-telegrambot/raw/main/luci-app-telegrambot_1.0.4_all.ipk)
opkg install /tmp/telebot.ipk
rm /tmp/telebot.ipk
/etc/init.d/bot enable
/etc/init.d/bot start
