# Використовуємо офіційний образ Python
FROM python:3.10

# Встановлення робочої директорії
WORKDIR /app

# Копіюємо файли проекту до контейнера
COPY . .

# Встановлюємо залежності
RUN pip install --no-cache-dir --upgrade pip \
    && pip install --no-cache-dir -r requirements.txt

# Відкриття порту 8000 для доступу до застосунку
EXPOSE 8000

# Команда для запуску FastAPI застосунку
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
