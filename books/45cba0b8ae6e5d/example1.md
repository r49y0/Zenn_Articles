---
title: "config.yaml"
---

https://zenn.dev/zenn/articles/zenn-cli-guide#cli-%E3%81%A7%E6%9C%AC%EF%BC%88book%EF%BC%89%E3%82%92%E7%AE%A1%E7%90%86%E3%81%99%E3%82%8B

# yaml summary

title : 本のタイトルを入力します
summary : 本の紹介文を入力します。これは有料の本であっても公開されます
topics : トピック（タグ）を 5 つまで指定します
published : 公開する場合はtrueにします
price : たとえば本を 1000 円で販売するときはprice: 1000と記載します（200〜5000 の間で 100 円単位で設定する必要があります）
chapters : チャプターの並び順を配列で指定します（入れ子には未対応）。ここに指定されなかったチャプターは zenn.dev に同期されません
toc_depth : 以下の説明をご覧ください