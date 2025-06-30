# 베이스 이미지
FROM python:3.10-slim

# 작업 디렉토리 설정
WORKDIR /app

# 의존성 설치를 위한 requirements.txt만 먼저 복사
COPY requirements.txt .

# 의존성 설치
RUN pip install -r requirements.txt

# 나머지 전체 소스 복사
COPY . .

# 컨테이너 실행 시 FastAPI 앱 실행
# CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
CMD ["fastapi", "run", "main.py"]
