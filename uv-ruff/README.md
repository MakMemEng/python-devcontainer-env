- Doc: https://zenn.dev/dena/articles/python_env_with_uv
- Doc: https://gihyo.jp/article/2024/03/monthly-python-2403

`uv venv`

`uv python pin 3.11`
`uv python install`

`source ./venv/bin/activate`
`deactivate`

`uv pip install pandas --no-cache`
`uv pip install ruff`

### requirements.txt
`uv pip install -r requirements.txt`
- 仮想環境にインストールされているパッケージバージョンの情報をrequirements.txtに同期
`uv pip sync requirements.txt`

### pyproject.toml
- pyproject.tomlを生成するコマンドはuvに存在しない
- pyproject.tomlに`dependencies`が存在すれば`uv sync`で同期することができる。

`uv sync`

- pyproject.tomlを使用したパッケージのインストール
`uv pip install -r pyporject.toml`
