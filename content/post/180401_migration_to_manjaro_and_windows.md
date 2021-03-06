---
title: "個人開発PCをManjaro LinuxとWindowsのデュアルブートにしてみた"
description: "個人開発PCをManjaro LinuxとWindowsのデュアルブートにしてみたので、それについてつらつら語っています。"
date: 2018-04-01T20:09:01+09:00
categories:
  - 雑談
tags:
  - Linux
  - 開発環境
draft: false
---

2016年に今のPC(ThinkPad X260)に買い換えてからずっとUbuntuを入れて使っていたのですが、少し飽きが来ていたのもあり、気分転換したくてOSを入れ替えました。今回はManjaro LinuxとWindowsとのデュアルブートです。

### Manjaro Linuxとは？

Arch LinuxベースのLinuxディストリビューションの一つです。
Arch Linuxはデスクトップ環境として使えるようになるまで自分でセットアップを頑張らなければいけない部分が多いのですが、Manjaro Linuxでは最初から十分なデスクトップ環境が整っています。

[公式: https://manjaro.org/](https://manjaro.org/) (ちなみに4/1はエイプリルフールデザインで突然のブルースクリーンでビビらされました)

Arch Linuxと同じくローリング・リリースモデルを採用しており、日々のアップデートを重ねてコアシステムを新しくしていくスタイルです。

パッケージ管理もArch Linuxと一緒でpacmanを使います。ガンガン新しいパッケージをリリースするArch Linuxの公式リポジトリですが、Manjaro公式リポジトリではArch Linuxからワンテンポ遅らせて安定してからパッケージをリリースします。WikiによるとArchのstableとManjaroのstableのラグは2週間ほどらしいです。

また、Arch Linuxの公式ではない一般ユーザが作成したパッケージリポジトリのAUR(Arch User Repository)はManjaroでも使用可能(これが強力)。

### Manjaroを選んだ理由は？

- ローリング・リリースモデルで育てていく感じが愛着持てそうだった
- Archに比べた圧倒的お手軽感
- **「新しいものをどんどん出していくが、少し落ち着いてから」という公式リポジトリのサイクルのリリースサイクルが自分の性に合ってた**

最後が自分的に一番ハマったポイントかなと思います。

### 他のディストリビューションは考えなかった？

Manjaroを知るまでは、Arch LinuxとLinux Mintで迷ってました。両極端。  

Archに挑戦してみたい気持ちはあったのですが、ちょっとVirtualBoxで試したところ先が長くなりそうで諦めました。気分転換に割ける時間で収まりそうになかったです。  
Mintは気分転換にはちょうど良さそうなお手軽感ではあったのですが、どうせ数カ月後には新しいLTSが出るんだろうなというタイミングだったので微妙感がありました。

### Manjaro入れてみてどう？

まだ運用し始めたばかりなのでなんともですが、新しいものが揃っている公式リポジトリがUbuntuに比べて超強力だなと思っています。Docker,Vagrant,Atom,Hugo,etc...が公式リポジトリからpacmanコマンド一発で新しめのものが手に入りました。  
あとAURが神です。
いつも開発に使っている一通りのツール群が全てカバーされていました。  
IntelliJとかVSCodeとかDropboxとか全部AURヘルパー(trizen使ってます)のコマンド一発でインストールできちゃうという。

動作の安定性に関してはまだこれからの運用の中での判断なのでなんともいえないですが、それも大丈夫なのであれば最高のOSですね。

### そういえばなぜ今になってWindowsとのデュアルブート？

たまーにWindowsがないと不便なケースが発生していたので。  
動作確認とか、VPN繋ぎたいときとか(LinuxをVPNクライアントとして使うの中々骨が折れる…)。


あと、1年前からWallpaper Engine使ってみたいと思ってた(↓)

{{< figure src="/images/18/04/01/miku.png" >}}

X260、これからもよろしくやで。
