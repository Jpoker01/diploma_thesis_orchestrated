FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .

RUN python -m pip install -U pip setuptools wheel 
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD ["uvicorn", "main:app", "--reload"]
