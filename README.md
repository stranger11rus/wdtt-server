# WDTT Server — готовый сервер за 1 минуту

Работает на любом VPS с Linux x86_64.

## Установка (Debian/Ubuntu)
```bash
curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/install.sh | bash
```

## Ручная установка
```bash
wget https://github.com/stranger11rus/wdtt-server/raw/main/wdtt-multi -O /usr/local/bin/wdtt-multi
chmod +x /usr/local/bin/wdtt-multi
mkdir -p /etc/wdtt
/usr/local/bin/wdtt-multi --listen 0.0.0.0:56000 --wg-port 56001 --listen-raw 0.0.0.0:56002 --password ПАРОЛЬ --admin ID --bot-token ТОКЕН
```

## Ключи
--listen — порт DTLS (56000)
--wg-port — WireGuard (56001)
--listen-raw — Raw режим (56002)
--password — пароль владельца
--admin — Telegram ID
--bot-token — токен бота

## Порты
56000 DTLS | 56001 WG | 56002 Raw

## Обновление
```bash
wget https://github.com/stranger11rus/wdtt-server/raw/main/wdtt-multi -O /usr/local/bin/wdtt-multi && chmod +x /usr/local/bin/wdtt-multi && systemctl restart wdtt
```