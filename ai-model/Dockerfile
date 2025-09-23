FROM python:3.9-slim

WORKDIR /app

# Установка зависимостей (PyTorch, Transformers, и т.д.)
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Копирование кода модели и скриптов обучения
COPY . .

# Команда для запуска скрипта обучения или сервера модели
CMD ["python", "train_or_run.py"]