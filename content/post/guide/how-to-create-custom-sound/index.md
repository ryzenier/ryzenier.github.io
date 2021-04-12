---
title: フィルター用独自サウンドの作り方
description: 時々聞かれるので自分のやっている方法を紹介します。
date: 2021-04-06
slug: guide/how-to-create-custom-sound
categories:
    - 攻略解説
tags:
    - 上級者向け
    - 超上級者向け
draft: false
image: voice-download.png
---

独自のサウンドを作る方法は、オンラインのサイトを使う方法もありますが、それだと遅いので、ここでは `voice.exe` を使った方法を紹介します。

## 1. `voice.exe` をダウンロード

下記のページにアクセスして「`voice.exe`」をダウンロードして好きなフォルダに入れます。

- https://www.elifulkerson.com/projects/commandline-text-to-speech.php

![voice.exe](voice-download.png)


## 2. コマンドプロンプトからコマンドを実行する

コマンドプロンプトを起動して `voice.exe` をダウンロードしたフォルダに移動します。

※やり方がわからない場合は「 `コマンドプロンプト フォルダ 移動` 」等でググってください。

移動したら↓のコマンドをコピペして、実行すると `voice.exe` と同じフォルダに `trans.wav` というファイルができます。

```
voice -n "Microsoft Zira Desktop" -o trans.wav trans
```

後は、いつもどおり「 `C:\Users\ryzenier\Documents\My Games\Path of Exile` 」に `trans.wav` を置いて完了です。


今回は例として「 `trans` 」にしましたが「 `blue blue green` 」のように複数単語にしたい場合は、↓のようにすることで、作成できます。

```
voice -n "Microsoft Zira Desktop" -o bbg.wav blue blue green
```
