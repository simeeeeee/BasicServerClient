FROM python:3.10-slim

# docker 파일 완성하기

# OS에 필요한 파일 옮겨오기

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD ["python", "-u", "run_client.py"]



