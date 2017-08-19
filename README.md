# 本番環境構築（雑）

```
git clone http://github.com/solt9029/Works
cd Works
mkdir docs
cd docker.works
docker-compose build
docker-compose up -d
docker exec -it dockerworks_web_1 bash
cd /var/www/html
npm install
npm run build
```