# verdaccio-docker-compose
verdaccio docker-compose 配置

## 使用
- 关闭本地 nginx，防止 80 端口冲突
```
sudo nginx -s stop
```
- 修改绑定 host
```
127.0.0.1  registry.npm.com
```
- 启动 docker 服务
```
docker-compose up -d
```
- 浏览器打开查看
  - http://registry.npm.com/
- 修改 .npmrc 配置
```
registry=http://registry.npm.com/
```

## 链接
- https://verdaccio.org/
  - https://verdaccio.org/docs/ssl
