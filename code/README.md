# サンプルコード

授業中に扱うコードとノートブックを置きます。回に対応するものは `lectures/` 側の番号と揃えてください（例: `03_ode_solvers.ipynb`）。

## 実行方法

リポジトリ直下で仮想環境を有効化してから実行します。

```bash
source .venv/bin/activate
python code/your_script.py
```

ノートブックの場合:

```bash
jupyter lab
```

## ノートブックを commit する前に

出力セルを消してから commit すると差分が読みやすくなります。

```bash
jupyter nbconvert --clear-output --inplace code/your_notebook.ipynb
```
