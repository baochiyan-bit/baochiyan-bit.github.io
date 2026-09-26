# baochiyan-bit.github.io（app-ads.txt 用）

AdMob は、App Store に登録した「デベロッパの Web サイト」の**ドメイン直下**にある `app-ads.txt` を確認します。
`https://baochiyan-bit.github.io/apps/` はサブフォルダなので、ドメイン直下（`https://baochiyan-bit.github.io/app-ads.txt`）に置くために、このリポジトリを別に作ります。

## 手順

1. AdMob →「アプリ」→ 対象アプリ →「app-ads.txt」に表示される1行をコピーして、`app-ads.txt` の2行目と置き換える（1行目のコメントは消してよい）
2. GitHub で **`baochiyan-bit.github.io`** という名前の Public リポジトリを作る（名前はこのとおりにする）
3. このフォルダを push する

   ```bash
   cd ~/Desktop/Claude\ Project/baochiyan-bit.github.io
   git init && git add . && git commit -m "app-ads.txt"
   git branch -M main
   git remote add origin https://github.com/baochiyan-bit/baochiyan-bit.github.io.git
   git push -u origin main
   ```

4. リポジトリの Settings → Pages で、Branch を **main / (root)** にして Save
5. `https://baochiyan-bit.github.io/app-ads.txt` が表示されるのを確認
6. App Store Connect のアプリ情報で「マーケティング URL」または「サポート URL」のドメインを `baochiyan-bit.github.io` にしておく（`https://baochiyan-bit.github.io/apps/hensai/support.html` でよい）

`index.html` は、トップにアクセスした人を `/apps/` に案内するためのものです。
