FROM --platform=linux/amd64 python:3.11-alpine

WORKDIR /book_catalog

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]
