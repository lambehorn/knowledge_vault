Docker — это программная платформа для разработки, доставки и запуска приложений в контейнерах.
### Ключевые особенности Docker:
- Изоляция - каждое приложение работает в своём [контейнере](Контейнер), не мешая другим.
- Портативность - [контейнере](Контейнер) можно запустить на любом сервере или компьютере с установленным Docker, независимо от ОС или конфигурации.
- Лёгкость - [контейнере](Контейнер) значительно «легче» виртуальных машин, так как не содержат целую операционная система, а используют ядро хоста.
- Управляемость - есть экосистема инструментов ([[Docker CLI]], [[Docker Compose]], [[Docker Hub]]) для сборки, хранения, развертывания и управления контейнерами.
### Установка Docker
#### на Ubuntu:
> примечание: в качестве shell рекомендуется использовать bash

1. Добавить репозитории Docker.

```bash
# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") stable" | \
sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
```

2. Установить пакеты Docker.

```bash
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

3. Проверить работает ли Docker тестовой [командой](Команда) hello-world

```bash
sudo docker run hello-world
```

