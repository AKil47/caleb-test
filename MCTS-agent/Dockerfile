FROM python:3.9-slim

WORKDIR /app

# Install dependencies first to leverage caching
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy all files from current directory
COPY . .

EXPOSE 5000

CMD ["python", "app.py"]
