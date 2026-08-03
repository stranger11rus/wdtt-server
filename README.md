# WDTT Server

## Установка
```bash
curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/deploy.sh | bash
```

## Порты
- 56000 — DTLS+TCP (основной)
- 56001 — WireGuard
- 56002 — Raw (до 200 Мбит/с)

## Raw режим
```bash
WDTT_RAW_PORT=56002 bash deploy.sh
```

## Переменные
WDTT_DTLS_PORT, WDTT_WG_PORT, WDTT_SSH_PORT, WDTT_RAW_PORT, WDTT_DIRECT_PORT, WDTT_ARGS

## Файлы
- deploy.sh — установщик
- wdtt-multi — бинарник сервера (x86_64)
