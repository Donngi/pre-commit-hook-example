# pre-commit example
gitのhooksを便利に扱うためのライブラリ[pre-commit/pre-commit](https://github.com/pre-commit/pre-commit)の設定サンプルリポジトリです。

https://github.com/pre-commit/pre-commit

## pre-commitコマンドそのもののインストール
homebrew
```shell
brew install pre-commit
```

python
```shell
pip install pre-commit
```

See more: [pre-commit: Installation](https://pre-commit.com/#install)

## 各リポジトリごとの設定手順
### STEP1: (設定ファイルがまだない場合)設定ファイル追加
```shell
# スクラッチで設定する場合
touch .pre-commit-config.yaml

# 設定サンプルをベースにする場合
pre-commit sample-config > .pre-commit-config.yaml
```

### STEP2: .gitのhooksに追加
```shell
pre-commit install
```

## その他便利なコマンド

```shell
# 特定のhookのみ実行
pre-commit run [hook-id]

# すべてのファイルに対して、全hookを実行
pre-commit run --all-files
```

## Reference
[GitHub: pre-commit/precommit](https://github.com/pre-commit/pre-commit)
[pre-commit.com](https://pre-commit.com)