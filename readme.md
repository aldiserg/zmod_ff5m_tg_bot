# Description

This is helm chart repositoty for [zmod_ff5m_telegram_bot](https://github.com/ghzserg/zmod/wiki/Telegram_en). Read FAQ before install.
Tested only on the same network (without ssh keys)

# Changes before run

All changes what you need to do in configMapAsFile.data.telegram.conf selection:

```
server: 3D_printer_host:7125
bot_token: 1111111111:AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
chat_id: 111111111

host: http://3D_printer_host:8080/?action=stream
host_snapshot: http://3D_printer_host:8080/?action=snapshot
```

# installation

helm upgrade --install ReleaseName ./ -n namespace -f values.yaml
