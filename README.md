# What are problems in LN?

```
[ライトニングネットワークに足りない点]

・組み合わせの自由度が少ない
  ・2018年7月現時点では全てのLN機能が個々の製品にビルドインされている。現時点だと労力を集約させることが効率的だが、個々のレイヤーごとに別々の製品になったほうが自由競争が起こりやすく組み合わせが増えやすい。
  ・https://image.slidesharecdn.com/lightningecosystemhashhub20180721-180721222107/95/lightninghashhub-conference-2018-18-638.jpg?cb=1532211725
・スマホがLNノードになれない
  ・2018年7月現在、ネットワークは熱狂者たちによって作られており、ビットコインのP2Pネットワークを参考にするとせいぜい数万ノードが最大数であり、それほど取引処理数は増やせない。
  ・これだと、理想的に見て25万TX/s(10000ノード / 4ノード/route * 100TX/s/route)、実際は10万TX/sが限度。
  ・利用用途としてはこれは十分な数とも言えるが、機械が使う支払い方法としては足りない。クレジットカードの全世界での秒間最大風速が200万TX/sなので。
  ・Iotはまだ早いため、スマホをLNノード(ウォレットではなく)にするのが早い
・エンジニアの参入コストが大きい
  ・プロトコルをそれなりに理解しないといけない
  ・OSI参照モデルのアプリケーション層に相当するプロトコルがあったほうがいい
・outsourcing watchtower, backupのインセンティブ、分散委任技術

ルーティングアルゴリズム関係
・安定的な仲介ノードの選定方法
・特定のノードに依存しにくい安定なペイメントルートを作るための動的ネットワーク構成方法(例:shitcoin.com)
・送金仲介手数料の最大化(送金にLNを使いたいと思うくらいには安く、ネットワークに参加しようと思うくらいには高い)
  ・各ノードの信用度も加味すべきか。
  ・利用方法に応じてアルゴリズムを変えるべきか。

ルーティングアルゴリズム実装方法
・ルールベースアルゴリズムアプローチ
・機械学習アプローチ

LN外部ビジネス
・AIというか自律的に動くマシンおよびソフトウェア(自律的生活サポートなど)

参考
6/23ベルリン、ライトニングハックデー
https://bitcointechweekly.com/front/summary-of-the-bar-camp-session-at-the-2nd-lightninghackday-in-berlin--improving-the-autopilot-of-ln/
```
