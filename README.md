# WDTT Server — с пейсером (+40% скорости)

Готовый сервер для интернета через видеозвонки ВК.

```bash
curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/deploy.sh | bash
```

## Что нового
- Пейсер: устраняет потери пакетов
- Скорость до 60 Мбит/с
- Совместим с iOS и Android

## Порты
56000 DTLS | 56001 WG | 56003 Raw

## Обновление
```bash
wget https://github.com/stranger11rus/wdtt-server/raw/main/wdtt-multi -O /usr/local/bin/wdtt-server && chmod +x /usr/local/bin/wdtt-server && systemctl restart wdtt
```

С уважением, команда VK Turn | vkturn.ru
