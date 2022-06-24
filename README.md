# react-django-mysql-nginx

バックエンドに Django、フロントエンドに React（Nginx に設置）、DB に MySQL を用いた３層構造コンテナ基盤

## 初期インストール方法

### サーバ側プロジェクト初期化(Django)

```
docker compose run --rm backend sh -c "django-admin startproject config ."
docker compose run --rm backend sh -c "python manage.py startapp testapp"
```

### クライアント側プロジェクト初期化(React)

```
docker-compose run --rm frontend sh -c "npm install -g create-react-app && create-react-app ."
docker-compose run --rm frontend sh -c "npm run build"
```

### コンテナ起動

```
docker compose up
```

## 起動確認

### サーバ側(Django)

http://localhost:8000/

### フロント側(React)

http://localhost/
