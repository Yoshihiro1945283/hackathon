# Nodeのベースイメージを使用
FROM node:16

WORKDIR /app

# 必要なファイルをコピーしてインストール
COPY package.json package-lock.json ./
RUN npm install

# ソースコードをコピー
COPY . .

# ビルド
RUN npm run build

# サーバー起動
CMD ["npm", "start"]
