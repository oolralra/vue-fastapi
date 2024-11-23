FROM python:3.10-slim

WORKDIR /app
# 소스코드가 복사될 디렉토리 생성

ADD requirements.txt .
# 라이브러리 목록 복사

RUN pip install --no-cache-dir -r requirements.txt
# 설치후 찌꺼기 삭제

ADD . . 

CMD ["uvicorn","main:app","--host","0.0.0.0","--port","8000"]
