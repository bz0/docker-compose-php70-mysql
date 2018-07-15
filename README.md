# docker-compose-php70-mysql
Docker-ComposeによるPHP7.0+MySQL5.7構築

# 使い方

## docker-compose.ymlの修正

PHPの「volumes」の指定を「- [ホスト側のディレクトリ]:/var/www/html」と修正します。  
  
コンテナは永続化されないので、コンテナを削除するとコンテナ内で作成したファイルも消えるため  
ホスト側にファイルを置き、そのディレクトリをコンテナ側から参照する手法を取ります。  
  
DBは、名前付きデータボリュームを、docker-compose.ymlで設定しているので修正不要です。

## php70-mysql環境の構築
Docker、Docker-Composeのインストールをしたら、このプロジェクトのカレントディレクトリで下記コマンドを実行して下さい。  

```bash
# docker-compose up -d
```
