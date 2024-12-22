# PHP 実行環境の構築手順
1. compose.yml ファイルの確認  
まず、プロジェクトディレクトリ内に `compose.yml` ファイルが存在するかを確認してください。
```bash
$ ls
README.md       compose.yml     docker          src
```

2. コンテナの起動  
以下のコマンドを実行し、コンテナをバックグラウンドで起動します。
```bash
docker compose up -d
```

3. コンテナへの接続  
コンテナ内で作業を行う場合は、下記コマンドでコンテナに接続してください。
```
docker exec -it php83_container bash
```

4. Hello Worldプログラムを実行  
サンプルとして用意されている PHP ファイル（sample.php）を以下のコマンドで実行します。
```bash
php sample.php
```
