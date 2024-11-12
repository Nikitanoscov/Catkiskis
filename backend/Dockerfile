# Основой слой 
FROM python:3.9

# Создаем и переходим в директорию
WORKDIR /app
# Подключаем скачиваем gunicorn
RUN pip install gunicorn==20.1.0

# Копируем с локального устройства файл с зависимостями
COPY requirements.txt .

# устанавливаем зависимости без сохранения кеша
RUN pip install -r requirements.txt --no-cache-dir

# Скопировать всё необходимое содержимое 
# той директории локального компьютера, где сохранён Dockerfile,
# в текущую рабочую директорию образа — /app.
COPY . .

# При старте контейнера запустить сервер разработки.
CMD ["gunicorn", "--bind", "0.0.0.0:8000", "kittygram_backend.wsgi"]