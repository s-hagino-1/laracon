# ユニットテスト実行手順

1. コンテナを起動させる
```
cd docker
docker compose up -d
```

2. コンテナに入る
```
docker exec -it docker-laracon-1 /bin/sh
```

3. composer install
```
cd /laracon
composer install
```

4. ユニットテスト実行
```
cd /laracon
vendor/bin/phpunit tests
```