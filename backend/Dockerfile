# Pythonのベースイメージを使用
FROM python:3.9-slim

WORKDIR /app

# 必要なファイルをコピーして依存関係をインストール
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .

CMD ["python", "app.py"]
