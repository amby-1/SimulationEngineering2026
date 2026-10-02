# 環境構築手順

## 1. Python の準備

Python 3.10 以降を使います。インストール済みかどうかは次で確認できます。

```bash
python --version
```

## 2. リポジトリの取得

```bash
git clone <このリポジトリの URL>
cd SimulationEngineering2026
```

## 3. 仮想環境の作成とパッケージのインストール

macOS / Linux:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Windows (PowerShell):

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## 4. 動作確認

```bash
python -c "import numpy, scipy, matplotlib; print('ok')"
```

`ok` と表示されれば準備完了です。Jupyter を使う場合は `jupyter lab` で起動します。

## よくあるつまずき

- **`pip install` が失敗する**: `pip install --upgrade pip` を実行してから再試行してください。
- **グラフが表示されない**: ノートブックでは `%matplotlib inline`、スクリプトでは `plt.show()` が必要です。
- **仮想環境が有効か分からない**: プロンプト先頭に `(.venv)` が付いているか確認してください。
