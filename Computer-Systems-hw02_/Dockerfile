# Використовуємо базовий образ Python
FROM python:3.8-slim

# Встановлюємо залежності за допомогою pip
COPY requirements.txt /app/requirements.txt
RUN pip install --no-cache-dir -r /app/requirements.txt

# Копіюємо вихідний код застосунку у робочу директорію /app
COPY . /app
WORKDIR /app

# Запускаємо застосунок
CMD ["python", "main.py"]