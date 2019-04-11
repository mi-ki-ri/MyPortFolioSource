+++
title: NadeNadeSynth
+++

URL: [https://nadenadesynth.herokuapp.com/](https://nadenadesynth.herokuapp.com/)

NadeNadeSynth(ナデナデシンセ)とは、画面を撫でることで座標に応じた音が出るWebアプリです。

技術的には、[Tone.js](https://tonejs.github.io/)を使っています。

フレームワークはNuxt.jsでデプロイ先はherokuです。

難しかった点として、Nuxtの強みであるはずのSSRがaudiocontextを複雑にしてしまったことがあります。

no-ssrタグを利用して解決したはずです。
