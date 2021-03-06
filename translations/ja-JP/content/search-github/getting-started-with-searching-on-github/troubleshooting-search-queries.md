---
title: クエリ検索のトラブルシューティング
intro: '{% data variables.product.product_name %} での検索中に予期しない結果が起きた場合、よくある問題および制限を確認することでトラブルシューティングできます。'
redirect_from:
  - /articles/troubleshooting-search-queries
  - /github/searching-for-information-on-github/troubleshooting-search-queries
  - /github/searching-for-information-on-github/getting-started-with-searching-on-github/troubleshooting-search-queries
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
topics:
  - GitHub search
shortTitle: Troubleshoot search queries
---

## タイムアウトの可能性

いくつかのクエリは、弊社の検索インフラで実行するには計算するうえでコストが高くなります。 皆さんが検索を迅速に行えるように、個別のクエリを実行する時間について制限を設けています。 まれなことですがクエリが制限時間を超えた場合、検索結果はタイムアウトになる前に見つかった全てのマッチを表示し、タイムアウトが起きたことを知らせます。

タイムアウトになったことは、必ずしも検索結果が未完了であるということではありません。 ただ、すべての検索可能なデータを検索する前にクエリが中断したことを意味しています。

## クエリの長さの制限

{% data variables.product.product_name %} での検索では、クエリの長さに一定の制限があります。

* 256 文字を超えるクエリはサポートされません。
* 6 つ以上の `AND`、`OR` や `NOT` 演算子を使ったクエリを作成することはできません。

コードの検索など特定の検索形式は、さらなる制限がある可能性があります。 詳しい情報については、これらの検索形式のドキュメントを確認してください。

## 参考リンク

- "[GitHub での検索について](/search-github/getting-started-with-searching-on-github/about-searching-on-github)"
