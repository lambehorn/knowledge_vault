Это панель управления для [[XRay]], которая облегчает настройку прокси-сервера. 

Marzban добавляет веб-интерфейс и управление пользователями, чтобы:
* создавать и удалять юзеров
* генерировать подписки для клиентов (например, для v2rayNG, Clash и других)
* смотреть статистику трафика
* управлять портами и прокси-настройками.

Настройка Marzban через [[Docker]]:
> примечание: действия происходят уже в скачаном [[Docker]]
> так же для сервера должны быть подготовлены  [[ssl]] сертификаты

1.  Подключаемся к серверу и скачиваем Marzban с официального репозитория.

```bash
sudo bash -c "$(curl -sL https://github.com/Gozargah/Marzban-scripts/raw/master/marzban.sh)" @ install
```

2.  Создаем админа.

```bash
marzban cli admin create --sudo
```

## Tips & tricks

Запрос на получение  admin token
```bash
curl  -kX POST "https://highwayvpn-latvia.duckdns.org:8000/api/admin/token" \
           -H "Content-Type: application/x-www-form-urlencoded" \
           -d "username=admin&password=admin"

```

Запрос на получение user info
```bash

```