# 実行までの手順

## 実行準備(コードのclone、仮想環境作成)
```bash
# 所望のディレクトリにcloneする
cd /share/(自分の名前ディレクトリ)
git clone https://github.com/rtmk0525/pytorch-sample.git
# 以下、仮想環境の構築（仮想環境名は`torch-sample`）
# anacondaのpathを通す
. /home/user?/set-anaconda.sh
# 仮想環境作成
conda create -n torch-sample python=3.11
# 仮想環境有効化
. activate torch-sample
# pythonライブラリをいくつかインストール
pip install torch torchvision ipykernel
```
## main.pyの実行手順
```bash
python main.py
```
## main.ipynbの実行手順
```bash
# jupyter notebookに仮想環境`torch-sample`を追加
# 参考: https://qiita.com/smiler5617/items/e0d9b3034d79457cc253
ipython kernel install --user --name=torch-sample
# jupyter notebook起動
jupyter notebook
```
以下、`main.ipynb`を開き、カーネル→カーネルの変更→`torch-sample`を選択し、実行する。
