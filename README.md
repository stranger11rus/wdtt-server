# WDTT Server

Готовый сервер для интернета через видеозвонки ВКонтакте.

## Быстрая установка
curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/install.sh | bash

## Ключи
--listen — порт DTLS (56000)
--wg-port — порт WireGuard (56001)
--listen-raw — порт Raw режима (56002)
--password — пароль владельца
--admin — Telegram ID админа
--bot-token — токен бота
--config-dir — папка конфигов

## Обновление
wget https://github.com/stranger11rus/wdtt-server/raw/main/wdtt-multi -O /usr/local/bin/wdtt-multi && chmod +x /usr/local/bin/wdtt-multi && systemctl restart wdtt
