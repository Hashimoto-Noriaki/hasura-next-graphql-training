# ベースイメージとしてNode.jsを使用
FROM node:20

# 作業ディレクトリを設定
WORKDIR /app

# 必要なファイルをコピー
COPY package.json yarn.lock ./

# 依存関係をインストール
RUN yarn install

# アプリケーションコードをコピー
COPY . .

# Metroサーバーのポートを公開
EXPOSE 8081

# 開発用サーバーを起動
CMD ["yarn", "start"]
