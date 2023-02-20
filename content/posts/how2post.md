---
title: "Hugoで生成されたサイトに新規投稿する方法"
date: 2023-02-20T21:34:12+09:00
draft: false
---

※以下の内容はGitHub Pagesを用いて公開を行っている場合の手順です．

1. [Hugo](https://gohugo.io/installation/)をインストールする(インストールしていない方のみ)
2. ローカルにリポジトリをクローンし，クローンしたディレクトリに移動する
3. `hugo new posts/ファイル名.md`を実行する
4. `content/posts/ファイル名.md`のtitleを書き換え，draftをfalseにする
5. 最終行に記事内容をMarkdown形式で書き込む
6. `hugo server`を実行し，`http://localhost:1313/`にアクセスして表示を確認する[※1]
7. 問題がなければコミットしてプッシュする

[※1]Hugoの設定ファイルに記述されているURLパスに従ってください．例えばこのサイトに関しては`http://localhost:1313/blog/`にアクセスする必要があります．