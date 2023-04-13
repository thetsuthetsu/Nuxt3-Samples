# Nuxt3ベーシックアプリケーション
## 参考
* https://reffect.co.jp/vue/nuxt3   

## setup
* https://nuxt.com/docs/getting-started/installation 

    ```
    5  npx nuxi init nuxt3app
    6  npm install

   11  cd nuxt3app
   12  npm run dev
   13  npm install
   14  npm run dev
   ```

## index page
1. pagesフォルダ作成
2. 新規ページ作成 pages/index.vue
3. app.vueに`<NuxtPage />`を追加
4. `localhost:3000`にアクセス

## about page
1. 新規ページ作成 pages/about.vue
2. `localhost:3000/about`にアクセス

## layouts作成
1. layoutsフォルダ作成
2. layouts/default.vueを作成
3. app.vue
    1. <NuxtLayout>
4. `localhost:3000` `localhost:3000/about`にアクセスし、共通のlayout.vueが表示されることを確認

## カスタムレイアウト
1. layouts/custom.vueを作成
2. pages/about.vueにdefinePageMetaを定義し、customレイアウトを指定。
4. `localhost:3000`にアクセスし、既定のレイアウトが表示されることを確認
5. `localhost:3000/about`にアクセスし、カスタムレイアウトが表示されることを確認

## フッター追加
1. layouts/footer.vueを作成し、名前付きslot(name="footer")を追加
2. app.vueに名前付き(name="footer")NuxtLayoutを追加

## コンポーネント追加
1. componentsフォルダ作成
2. components/Navbar.vueを作成
3. layouts/default.vueに`<Navbar />`コンポーネントを追加 （※自動インポート)


## Key Concepts
1. [Auto Imports](https://nuxt.com/docs/guide/concepts/auto-imports)

   
   
