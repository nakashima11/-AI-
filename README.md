# MNIST手書き数字認識プロジェクト

このプロジェクトは、PyTorchを使用したMNISTデータセットの手書き数字認識システムを実装したものです。CNNとLSTMを組み合わせたモデルを使用して高精度な数字認識を実現しています。

## プロジェクト内容

- **mnist_AI.ipynb**: モデルのトレーニングと評価を行うJupyterノートブック
  - CNN-LSTMハイブリッドモデルの定義
  - MNISTデータセットを使用したトレーニング
  - モデルの評価（精度約99%）
  - モデルの保存

- **mnist_game.ipynb**: 学習したモデルを使用したインタラクティブなアプリケーション
  - PyQt5を使用したGUIアプリケーション
  - ユーザーが数字を描画して認識するゲーム
  - リアルタイムでの手書き数字認識

- **cnn_lstm_mnist.pth**: 学習済みのモデルパラメータファイル

## 使用方法

1. `mnist_AI.ipynb` を実行してモデルをトレーニングするか、提供されている事前学習済みモデル `cnn_lstm_mnist.pth` を使用します
2. `mnist_game.ipynb` を実行して手書き数字認識ゲームを起動します
3. アプリケーション上で数字を描き、回答ボタンを押して認識結果を確認します

## 要件

- Python 3.x
- PyTorch
- torchvision
- numpy
- cv2 (OpenCV)
- PyQt5（ゲームアプリケーション用）

## モデル構造

このプロジェクトでは、畳み込みニューラルネットワーク（CNN）と長短期記憶（LSTM）を組み合わせたハイブリッドモデルを使用しています。モデルは次の層で構成されています：

1. 3つの畳み込み層（バッチ正規化、ReLU活性化、MaxPoolingを含む）
2. 3層のLSTM（隠れ層サイズ256）
3. 2つの全結合層

## 参考文献
https://qiita.com/DeepTama/items/379cac9a73c2aed7a082
https://qiita.com/dolce_itf/items/be85244a31654d1d56ef
https://colah.github.io/posts/2015-08-Understanding-LSTMs/


https://github.com/user-attachments/assets/52c36846-3ce2-4458-ab50-b2947e568e68

手書き数字認識
