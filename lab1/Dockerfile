FROM python:3.11-slim

WORKDIR /app

COPY . ./lab1

RUN pip install --no-cache-dir -r lab1/requirements.txt

ENV PYTHONPATH=/app:/app/lab1

CMD ["uvicorn", "lab1.main:app", "--host", "0.0.0.0", "--port", "8000"]