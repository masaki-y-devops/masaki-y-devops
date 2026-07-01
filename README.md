### TL; DR

数年前からLinux（Arch/Gentoo/NixOS）のスクラッチ構築や自動化に熱中し、

雑多なコードをプライベートなクラウドストレージに蓄積していました。

現在はAIをペアプロ相手として使い、[Next.js+Vercelでの爆速開発](https://github.com/masaki-y-devops/portfolio-sites-react)や[WPFでの定型作業効率化ツールを自作](https://github.com/masaki-y-devops/iso-builder-wpf)しています。

「トイル（手作業）を技術で撲滅し、仕組みで生産性を加速させる」仕事がしたい人間です。

### 【個人活動・システム運用実績】
[Linux（Arch, NixOS）を用いたOS環境の自動構築・整備](https://github.com/masaki-y-devops/nixos-setup-flakes)や、

[Ubuntu Serverで自宅サーバーの構築およびマルチコンテナ環境の運用の経験](https://github.com/masaki-y-devops/self-hosted-docs)があります。

単にツールを動かすだけでなく、インフラの再現性（**IaC**類似の思想）や、

運用の自動化（**SRE**のような考え方）を意識した設計・トラブルシューティングが強みであると自負しています。

ポートフォリオ（兼、実験場・playground）サイトはこちら→[masaki-y-devopsの遊び場](https://portfolio-sites-react.vercel.app/)

_"Thanks for your visiting (and of course following)! I'm still (or may be forever) a beginner programmer in Japan, so I'm happy that my code has reached to you. Happy coding!"_

<details>
<summary> <strong>詳しいスキルセットや経歴を見る（クリックで展開）</strong> </summary>

#### 1. マルチコンテナ環境の構築とトラフィック制御
- **Docker Composeを用いた運用：** Nextcloud、WordPress、FreshRSS、changedetection.ioなど、特性の異なる複数のWebアプリケーションのマルチコンテナ環境を設計・構築。ボリュームマウントやコンテナ間ネットワークの分離の概念を学習しました。
- **Apacheリバースプロキシの配置：** changedetection.ioの運用では、TailscaleのMagicDNS機能を用いたSSL接続を可能とするため、コンテナの前段にApacheを配置して実装。HTTPヘッダーの制御やWebネットワークのプロトコルへの理解の素養を培いました。

#### 2. 運用の自動化（トイル削減）とセキュリティ
- **SSL証明書の自動更新：** メンテナンスコスト（手作業のトイル）を削減するため、Certbotやtailscale利用環境でのSSL証明書発行・更新タスクを完全に自動化し、低運用コストな環境を構築。
- **システムアップデートの自動化**: インタラクティブな対応が必要で予期せぬ停止をしていたサーバーをいち早く発見し、スクリプトの調整でアップデートの停止時間を最小限に抑えました。Ubuntu Pro ESMも適用し、セキュリティを高めていました。

#### 3. OSレイヤーにおけるトラブルシューティング能力
- **systemd起動問題の解決：** サーバー起動時におけるミドルウェアやサービスの起動順序の問題に直面した際、systemctl等を用いた状態分析から原因を特定。ユニットファイルのカスタマイズによって自動起動の安定化を解決しました。
- **先進的OSの検証：** NixOS flakesを用いた「宣言的な設定管理（環境の再現性担保）」や、Arch Linuxの構築を通じたLinuxカーネル・パッケージのシンプルな構成（EFISTUB,iwd,systemd-networkd,xinit+i3wm,swayなど)への知見を養いました。

#### 4. 複数パラダイムの言語習得
- C#やTypeScirptを用いたアプリケーション開発に加え、Nix, Haskell（純粋関数型言語）の基礎の学習を通じて、型安全で堅牢なシステム設計の思想を習得。Pythonを用いた自動化スクリプトの作成など、必要に応じた柔軟な言語選定に努めています。

#### 5.【趣味・ガジェット/ハードウェアへの関心】
ハードウェアの物理構造、リソース制限下での最適化、および低レイヤー（OS/カーネル）のチューニングに強い関心があります。

自作PC・UMPCのカスタマイズ： ハードウェアの仕様（TDP、排熱、アーキテクチャ）に関心があり、小型筐体におけるリソースの最適化を楽しんでいます。OSのチューニング： UMPCや自宅サーバーにArch LinuxやNixOSを導入し、ハードウェアの性能を最大限に引き出すためのミニマルな環境構築やカーネル設定、自動化スクリプトの作成を趣味として行っています。

- **UMPC（超小型PC）の活用と最適化：**
  GPD WIN 2、GPD WIN Mini（2024）、GPD MicroPCなどを所有。極小の筐体における排熱・TDPの制御や、Linux（Arch/NixOS）を導入した際のハードウェア認識、カーネルパラメータの最適化を自ら楽しんでいます。特にMicroPCを用いたシリアル通信やネットワークの足回りといった「物理レイヤー」への関心も高いです。
- **目的特化型の自作PC/自宅サーバー構築：**
  「i3-12100F」をベースに、高速I/Oを理由に選定した「WD Black SN850X」、過剰なほどの給電安定性と冗長性を持つ電源「CORSAIR RM1000e」を組み合わせた自宅サーバー（Ubuntu Server/Docker Compose）を構築。過去のi9ハイエンド環境のパーツ資産を「安定性とI/Oパフォーマンス」に全振りした構成へ再配分するなど、限られたリソースを最適化するキャパシティプランニングをプライベートでも実践しています。

</details>
