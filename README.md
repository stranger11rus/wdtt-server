# WDTT Server

curl -sSL https://raw.githubusercontent.com/stranger11rus/wdtt-server/main/deploy.sh | bash

## Порты
56000 DTLS | 56001 WG | 56002 Raw

## Raw режим
WDTT_RAW_PORT=56002 bash deploy.sh

## Обновление
wget https://github.com/stranger11rus/wdtt-server/raw/main/wdtt-multi -O /usr/local/bin/wdtt-server && chmod +x /usr/local/bin/wdtt-server && systemctl restart wdtt