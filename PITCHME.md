# 成果報告(yuki)
---
## 今日の作業
類似画像検索の試作
 - どうやって実装するか調べる
 - 試しに動かしてみる
---
## やり方
 - 特徴点マッチングを利用する方法
 - ** DeepLearning(転移学習) **　←　これやってみる
 - DeepLearning(転移学習+ファインチューニング)
 - 他もいろいろあるはず・・
---
## 転移学習
- すでに学習済みのモデルを別領域で使う方法
- 学習データとか用意しなくてよくて手軽
- (↓)メルカリさんのブログから拝借  
![aa](https://cdn-ak.f.st-hatena.com/images/fotolife/k/kumonworld/20171219/20171219155957.png)
---
## 実装
- chainer(python)
- 主要なモデルが用意されてる。  
(VGG16, GoogLeNET, ResNETなど)  
- 流れ
  - 特徴抽出：↑のモデルにデータを通す。最終手前のレイヤの出力をもらう
  - 類似度算出：特徴(ベクトル)を比較。(コサイン類似度＝向きが近いと似てる)
---
## どうだったか


やったこと
