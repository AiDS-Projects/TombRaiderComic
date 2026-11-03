# 部署文档 - 第一集视频简报：定 Mode 与剧情定位

## 本地预览

- 预览地址: http://localhost:8000/api/projects/PRJ-20261102-205a67/preview/dev/index.html

## 部署步骤

1. 构建镜像: `docker build -t app .`
2. 启动服务: `docker-compose up -d`
3. 健康检查: `curl http://localhost:8000/api/health`
