# WDTT Server — Raw + Pacer

Сервер для интернета через видеозвонки ВКонтакте. Полностью совместим с клиентами WDTT, qWDTT и VK Turn (iOS).

## Быстрая установка
```bash
curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/deploy.sh | bash
```bash
cd /root/wdtt-server-repo && cat > README.md << 'EOF'
# WDTT Server — Raw + Pacer

Сервер для интернета через видеозвонки ВКонтакте. Полностью совместим с клиентами WDTT, qWDTT и VK Turn (iOS).

## Быстрая установка
```bash
curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/deploy.sh | bash
```

Что нового в v1.4.3

· 🚀 Собран на Go 1.26 — upload вырос в 10 раз (до 20 Мбит/с на iOS)
· 📦 Пейсер (247 KiB/s) — +40% стабильности, без потерь
· 🔴 Raw (UDP) на порту 56003 — до 100+ Мбит/с с qWDTT
· 👥 Лимит пользователей: 1000
· 📊 Суточная статистика с лимитом 8 ГБ

Порты

Порт Протокол Клиенты
56000 DTLS iOS (VK Turn)
56001 WG UDP Android (WDTT)
56003 Raw UDP Android (qWDTT)

Ручное обновление

```bash
wget https://github.com/stranger11rus/wdtt-server/raw/main/wdtt-multi -O /usr/local/bin/wdtt-multi && chmod +x /usr/local/bin/wdtt-multi && systemctl restart wdtt
```

Контакты

· Поддержка: @vk_turn_support_bot
· Сайт: vkturn.ru

С уважением, команда VK Turn | vkturn.ru
