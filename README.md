# 機械学習ハンズオン（ML-HOL）

機械学習と深層学習の基礎から応用までを学ぶハンズオン形式の教材です。Jupyter Notebookを使用して、理論の解説と実装を同時に学ぶことができます。

## 概要

このリポジトリは、機械学習の基礎からディープラーニングの実践的なトピックまでをカバーする一連のJupyter Notebookを提供しています。各ノートブックは、理論的な説明とPythonによる実装を含み、インタラクティブに学習できるように設計されています。

## 学習内容

### 1. 機械学習の基礎（01_machine_learning_basics.ipynb）
- 機械学習の概要
- ニューラルネットワークの基本構造
- パラメータ学習の仕組み
- 分類問題と損失関数
- 誤差逆伝播法（バックプロパゲーション）
- 学習率と最適化手法
- 実践：簡単なニューラルネットワークの実装

### 2. 深層ニューラルネットワーク（02_deep_neural_networks_tutorial.ipynb）
- 深層学習の基本概念
- Kerasを使用したDNNの構築
- 正則化テクニック（L1/L2正則化、ドロップアウト）
- 高度な最適化アルゴリズム
- モデル評価と可視化

### 3. 畳み込みニューラルネットワーク（03_cnn_tutorial.ipynb）
- CNNの基本構造
- 畳み込み層とプーリング層
- 画像分類タスク
- データ拡張（Data Augmentation）
- 転移学習（Transfer Learning）

### 4. リカレントニューラルネットワーク（04_rnn_basics.ipynb）
- RNNの基本概念
- 系列データの処理
- LSTM（Long Short-Term Memory）
- GRU（Gated Recurrent Unit）
- テキスト生成や時系列予測

## 対象者

- プログラミングの基礎知識を持つ方
- 機械学習やディープラーニングを体系的に学びたい方
- 理論だけでなく実装も学びたい方
- データサイエンスやAI分野に興味のある方

## 前提知識

- Python の基本的な文法
- NumPy や Pandas の基本的な使い方
- 大学レベルの基本的な数学（微分・線形代数）の知識があると望ましい

## 環境セットアップ

環境のセットアップ方法については、[SETUP.md](SETUP.md) を参照してください。

## 学習の進め方

1. 順番にノートブックを実行することをお勧めします
2. コードセルを実行し、結果を確認してください
3. 説明を読んで理論を理解し、コードの実装方法を学んでください
4. 各ノートブックの最後にある練習問題に挑戦してみてください
5. パラメータを変更したり、独自のデータで試したりして実験してみてください

## 参考資料

- [Deep Learning](https://www.deeplearningbook.org/) by Ian Goodfellow, Yoshua Bengio, and Aaron Courville
- [Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow](https://www.oreilly.com/library/view/hands-on-machine-learning/9781492032632/) by Aurélien Géron
- [TensorFlow Documentation](https://www.tensorflow.org/api_docs)
- [Keras Documentation](https://keras.io/api/)

## ライセンス

このリポジトリのコードと資料は [MIT License](LICENSE) のもとで提供されています。

## 貢献

誤字脱字、コードの修正、ドキュメントの改善などの貢献を歓迎します。プルリクエストを送る前に、イシューで議論してください。