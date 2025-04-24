# 機械学習ハンズオン環境のセットアップ手順

このドキュメントでは、機械学習ハンズオン（ml-hol）のための環境セットアップ方法を説明します。

## 前提条件

以下のいずれかの環境を用意してください：

- Python 3.12以上のインストール済み環境
- Anaconda または Miniconda のインストール済み環境

## セットアップ方法

### 方法1: pipを使用する場合

1. リポジトリをクローンするか、ダウンロードします。

```bash
git clone <リポジトリURL>
cd ml-hol
```

2. パッケージをインストールします。

```bash
pip install -r requirements.txt
```

3. Jupyter Notebookを起動します。

```bash
jupyter notebook
```

または

```bash
jupyter lab
```

### 方法2: Anacondaを使用する場合

1. リポジトリをクローンするか、ダウンロードします。

```bash
git clone <リポジトリURL>
cd ml-hol
```

2. Conda環境を作成してアクティベートします。

```bash
conda env create -f environment.yml
conda activate ml-hol
```

3. Jupyter Notebookを起動します。

```bash
jupyter notebook
```

または

```bash
jupyter lab
```

## 環境の検証

環境が正しくセットアップされたことを確認するには、以下のPythonコードを実行してみてください：

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

### 一般的な問題

1. **TensorFlowのインストールに関する問題**
   
   Windows環境では、TensorFlowのインストールに問題が発生する場合があります。
   
   解決策: `pip install tensorflow` を個別に実行し、エラーメッセージを確認してください。

2. **japanize-matplotlibに関する問題**

   フォントが正しく表示されない場合は、以下を試してください：
   
   ```python
   import matplotlib.font_manager as fm
   print([f.name for f in fm.fontManager.ttflist])
   ```
   
   上記のコマンドで、利用可能なフォントを確認し、代替フォントを設定してください。

3. **メモリ不足エラー**

   ノートブックの実行中にメモリ不足エラーが発生した場合は、バッチサイズを小さくするか、データサンプルを減らしてみてください。

## 追加のリソース

- [Python公式ドキュメント](https://docs.python.org/)
- [Jupyter Notebookドキュメント](https://jupyter-notebook.readthedocs.io/)
- [TensorFlowドキュメント](https://www.tensorflow.org/api_docs)
- [scikit-learnドキュメント](https://scikit-learn.org/stable/)