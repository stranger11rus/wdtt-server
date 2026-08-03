# WDTT Server

Готовый сервер для интернета через видеозвонки ВКонтакте.
Работает на Debian, Ubuntu, CentOS.

## Установка

```bash
curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/deploy.sh | bash
```

После установки:
```bash
/usr/local/bin/wdtt-server --password ПАРОЛЬ --admin TELEGRAM_ID --bot-token ТОКЕН
```

- **ПАРОЛЬ** — любой пароль для шифрования
- **TELEGRAM_ID** — ваш ID (@userinfobot)
- **ТОКЕН** — токен бота (@BotFather)

## Порты

56000 DTLS | 56001 WG | 56002 Raw

## Raw режим

```bash
/usr/local/bin/wdtt-server --listen-raw 0.0.0.0:56002
```

## Обновление

```bash
wget https://github.com/stranger11rus/wdtt-server/raw/main/wdtt-multi -O /usr/local/bin/wdtt-server && chmod +x /usr/local/bin/wdtt-server && systemctl restart wdtt
```