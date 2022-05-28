# cape_ratio_survey
CAPEレシオについて調べた

# リンク
[SP500 PER](https://www.multpl.com/s-p-500-pe-ratio)
[超過CAPEについて](https://stock-marketdata.com/excess-cape-yield)
[ロバート・シラーのデータ](http://www.econ.yale.edu/~shiller/data.htm)

# Poetryの使い方

## install (uninstall)
https://qiita.com/makuramoto1/items/b3f4a0d610e4f97ef3f8

## init

`poetry init`をプロジェクト内で実行。まだプロジェクトファイルがない場合は`poetry new <pj_name>`で作成可能

## venvファイルをプロジェクトフォルダ内に作成

`poetry config virtualenvs.in-project true`

## 仮想環境をセットアップ

`poetry install # dev環境を除く場合は --no-dev`

## パッケージ追加

`poetry add <package_name>`

## poetryを動かす

```
poetry shell # 仮想環境に入る
poetry run <cmd> # cmdを仮想環境で実行
```

## pyproject.tomlを使ってpoetry.lockを更新する
これをやらない場合poetry installは.lockを参考にinstallする

```bash
poetry update --dry-run # 何が変更されるかを事前に検証すること
poetry update
```