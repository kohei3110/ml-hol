# 機械学習ハンズオン環境のセットアップ手順

このドキュメントでは、機械学習ハンズオン（ml-hol）のための環境セットアップ方法を説明します。

## 前提条件

以下の各ツールをインストールしてください：

- [Git](https://git-scm.com/downloads)
- [Docker](https://www.docker.com/)
- Visual Studio Code
   - 拡張機能 **Dev Containers** も併せてインストールしてください。

## セットアップ方法

1. リポジトリをクローンするか、ダウンロードします。

```bash
git clone https://github.com/kohei3110/ml-hol.git
cd ml-hol
```

2. VS Code を GUI から起動します。CUI で起動する場合は、以下のコマンドをターミナルから打ちます。

```bash
code .
```

3. VS Code 左下の青背景に白い字で「> <」のボタンを押下し、「Reopen in Container」を選択し、Dev Container を起動します。

## 環境の検証

環境が正しくセットアップされたことを確認するには、`00_setup.ipynb` を開き、以下のコードを実行します：

```python
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import sklearn
import tensorflow as tf
import japanize_matplotlib

# バージョン情報の表示
print(f"NumPy: {np.__version__}")
print(f"TensorFlow: {tf.__version__}")
print(f"scikit-learn: {sklearn.__version__}")
```

## トラブルシューティング

1. **メモリ不足エラー**

   ノートブックの実行中にメモリ不足エラーが発生した場合は、バッチサイズを小さくするか、データサンプルを減らしてみてください。

## 追加のリソース

- [Python公式ドキュメント](https://docs.python.org/)
- [Jupyter Notebookドキュメント](https://jupyter-notebook.readthedocs.io/)
- [TensorFlowドキュメント](https://www.tensorflow.org/api_docs)
- [scikit-learnドキュメント](https://scikit-learn.org/stable/)