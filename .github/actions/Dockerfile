# 1. Используем базовый образ. Alpine - очень легковесный.
FROM alpine:latest

# 2. Устанавливаем необходимые пакеты. В нашем случае это bash.
RUN apk add --no-cache bash

# 3. Копируем файл со скриптом внутрь контейнера.
COPY entrypoint.sh /entrypoint.sh

# 4. Делаем скрипт исполняемым.
RUN chmod +x /entrypoint.sh

# 5. Указываем, какая команда будет запускаться при старте контейнера.
ENTRYPOINT ["/entrypoint.sh"]