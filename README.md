# SimulationEngineering2026

シミュレーション工学（2026年度）の授業資料置き場です。講義スライド・サンプルコード・課題・データをまとめて管理します。

## ディレクトリ構成

| ディレクトリ | 内容 |
| --- | --- |
| `lectures/` | 回ごとの講義資料（スライド、ノート、板書など） |
| `assignments/` | 課題の説明と提出方法 |
| `code/` | 授業で扱うサンプルコード・Jupyter ノートブック |
| `data/` | 演習で使うデータファイル |
| `docs/` | シラバス、環境構築手順、参考文献などの補助資料 |

各ディレクトリの `README.md` に、その中身の扱い方を書いています。

## 環境構築

Python 3.10 以降を想定しています。

```bash
python -m venv .venv
source .venv/bin/activate   # Windows は .venv\Scripts\activate
pip install -r requirements.txt
```

Jupyter を使う場合は次のコマンドで起動します。

```bash
jupyter lab
```

詳細は [`docs/setup.md`](docs/setup.md) を参照してください。

## 更新の進め方

1. `main` から作業用ブランチを作る
2. 資料を追加・修正してコミットする
3. Pull Request を作成してレビュー後に `main` へマージする

資料の追加時は、ファイル名の先頭に回数（`01_`, `02_` …）を付けて並び順が分かるようにしてください。
