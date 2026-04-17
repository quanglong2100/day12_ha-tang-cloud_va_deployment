FROM python:3.11-slim

WORKDIR /app

# Vì mình sẽ để context là tại chỗ, nên chỉ cần COPY trực tiếp
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy file code và thư mục utils
COPY app.py .
COPY utils/ ./utils/

CMD ["python", "app.py"]