# next_sample

React でWEBアプリを作成する際のテンプレート

## ローカルへのコピー

以下を clone  
```bash
git clone https://github.com/cti1650/next_sample.git
```

## リポジトリを複製する

1. Git Bash を開いてください。

2. リポジトリのベアクローンを作成します。   
   ```bash
   git clone --bare https://github.com/cti1650/next_sample.git
   ```

3. 新しいリポジトリをミラープッシュします。(--mirror 以降は複製先のリポジトリを指定)  
   ```bash
   cd next_sample.git
   git push --mirror [複製先リポジトリURL]
   ```

4. 先ほど作成した一時ローカルリポジトリを削除します。  
   ```bash
   cd ..
   rm -rf next_sample.git
   ```
   
5. 先ほど作成した複製先のリポジトリをクローンします。  
   ```bash
   git clone [複製先リポジトリURL]
   ```
   
6. 必要な機能をインストールする。  
   ```bash
   npm install
   ```
   
7. 動作確認  
   ```bash
   npm start
   ```
   
   ブラウザで [http://localhost:3000/](http://localhost:3000/) を開く
   
8. デプロイ
   ```
   npm run deploy
   ```


This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.js`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/import?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
