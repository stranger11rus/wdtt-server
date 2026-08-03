# WDTT Server — готовый сервер за 1 минуту

Сервер для интернета через видеозвонки ВКонтакте. Работает на Debian, Ubuntu, CentOS.

## Установка

```bash
WDTT_ARGS="--password ПАРОЛЬ --admin TELEGRAM_ID --bot-token ТОКЕН" bash -c "$(curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/deploy.sh)"
```bash
cd /root/wdtt-server-repo

cat > README.md << 'EOF'
# WDTT Server — готовый сервер за 1 минуту

Сервер для интернета через видеозвонки ВКонтакте. Работает на Debian, Ubuntu, CentOS.

## Установка

```bash
WDTT_ARGS="--password ПАРОЛЬ --admin TELEGRAM_ID --bot-token ТОКЕН" bash -c "$(curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/deploy.sh)"
```

Где:

· ПАРОЛЬ — придумайте любой пароль (нужен для шифрования)
· TELEGRAM_ID — ваш Telegram ID (узнать у @userinfobot)
· ТОКЕН — токен бота (создать у @BotFather)

Порты

Порт Режим
56000 DTLS+TCP (основной)
56001 WireGuard
56002 Raw (до 200 Мбит/с)

Включить Raw

```bash
WDTT_RAW_PORT=56002 WDTT_ARGS="..." bash deploy.sh
```

Обновление

```bash
wget https://github.com/stranger11rus/wdtt-server/raw/main/wdtt-multi -O /usr/local/bin/wdtt-server
chmod +x /usr/local/bin/wdtt-server
systemctl restart wdtt
```

