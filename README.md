# このプロジェクトについて

# 前提
- Dockerおよびdocker-composeを利用できること

# ローカル環境構築

1. git clone このプロジェクトのクローンURL
2. cd triangle-demo
3. docker-compose up
4. ブラウザから`http://localhost:3000/`にアクセスする  
※docker-compose upから立ち上がるまでに1分程度待たないといけないです

# Webからアクセス
このアプリケーションはFirebase Hostingを利用してWeb上に公開しています。

https://triangle-demo-c574e.web.app/

からアクセスできます。

# アプリケーションの仕様

三角形の種類を判別するWebアプリケーションです。

三角形の各辺の長さを入力して計算するボタンを押すと三角形の種類をアラートに表示します。

下記の三角形を作れない場合の判定条件に合致する場合、三角形を作れませんと表示する。
条件: A辺+B辺 <= C辺、またはB辺+C辺 <= A辺、またはA辺+C辺 <= B辺

三角形を作れる場合の判定条件は以下として、それぞれ三角形の判定結果を表示する。
1. 3つの辺の長さが等しい場合、正三角形と表示する。
2. 2つの辺の長さが等しい場合、二等辺三角形と表示する。
3. 3つの辺の長さがどれも異なる場合、不等辺三角形と表示する。 

入力項目は以下の制約があります。
- 正の整数のみ
- 半角数字のみ
- 1~99まで

入力規則に違反する場合、違反した項目の下部に「1から99の整数を半角数字で入力してください。」というメッセージを表示します。

対応ブラウザは最新版のChromeです。

# 課題

以下コマンドのとおりにブランチを作成し、テストケースを作成してください。

`$ git branch feature/<your-name>`  
<your-name>は自身の名前のアルファベットに置き換えてください。  

`$ git checkout feature/<your-name>`  

`test`ディレクトリ配下に`<your-name>-testcase.md`ファイルを作成する。
  
`test`ディレクトリの`koyama-testcase.md`を参考にテストケースを作成してください。
  
テストケース作成後、以下コマンドでファイルをpushしてPRを作成してください。
  
`$ git add .`  
`$ git commit -m "自分で考えたコミットメッセージ"`  
`$ git push -u`

