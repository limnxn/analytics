# Environment setup for analytics

## Database
### ダンプファイルの自動インポート
```
$ cp yourdumpfile.sql /mysql/initdb.d
```

## Docker
### コンテナの起動
```
$ docker-compose up -d
$ OR docker-compose up {service} mysql -d
```

### データベースの接続
別コンテナからMySQLコンテナに接続するホスト名はサービス名を使います。  
`localhost`や`127.0.0.1`では接続エラーになるため注意してください。  

## Documents
- [Grafana Documentation](https://grafana.com/docs/grafana/latest/)
- [Metabase Documentation](https://www.metabase.com/docs/latest/)
- [What is Apache Superset?](https://superset.apache.org/docs/intro/)
