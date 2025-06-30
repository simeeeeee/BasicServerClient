FROM python:3.10-slim
WORKDIR /app
COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

EXPOSE 8000

CMD ["fastapi", "run","main.py"]

# ###
#
# 다음 주석을 지우고 docker 파일을 완성하자.
#
# ###