+++
title = "MyPortfolio"
+++


このページとこのページを動かしている仕組み全体のこと。

このページはGithub Pagesにてデプロイされています。

Github Pages へのデプロイはCircleCIを経由しています。

CircleCIが動くのは別リポジトリ( [MyPortFolioSource](https://github.com/mi-ki-ri/MyPortFolioSource) )にプッシュがあったときです。

つまり、

1. [MyPortFolioSource](https://github.com/mi-ki-ri/MyPortFolioSource)へのプッシュ
2. CircleCIが発動、
    - MyPortFolioSourceの中身を取ってきてhugo
    - [MyPortFolio](https://github.com/mi-ki-ri/MyPortFolio)(このページのリポジトリ)にプッシュ
    - (実は[テーマのリポジトリ](https://github.com/mi-ki-ri/MyPortfolioTheme)もあったり…)
3. Github Pagesが動いてデプロイしてくれる

という多層構造になっています。

なぜこうしたのかというと、Github上でファイルを作るだけで更新される仕組みにしたかったからです。
