# Backend Starter

一个面向 Web、H5、小程序、App 的 NestJS 后端起步仓库，内置本地 Docker 开发环境、Prisma、Redis、Swagger、Jest、GitHub Actions，以及单台阿里云服务器上的 `staging + production` 双环境部署方案。

## 技术栈

- NestJS + TypeScript
- PostgreSQL + Prisma
- Redis
- Swagger / OpenAPI
- Jest + Supertest
- Docker Compose
- GitHub Actions + GHCR
- Nginx

## 3 分钟快速启动

1. 安装 `Docker Desktop`、`git`，可选安装 `Node 22+` 和 `corepack`。
2. 克隆仓库后执行 `make init`。
3. 查看接口文档：`http://localhost:3000/docs`
4. 健康检查：`http://localhost:3000/health`
5. 打开演示网页：`http://localhost:3000/demo`
6. 默认管理员账号来自 `.env.local` 中的 `DEFAULT_ADMIN_EMAIL` 和 `DEFAULT_ADMIN_PASSWORD`

## 常用命令

- `make init`：初始化本地环境、执行 migration、注入种子数据
- `make up`：后台启动所有容器
- `make down`：停止本地环境
- `make logs`：查看 API 日志
- `make migrate`：执行 Prisma migration
- `make seed`：执行种子数据
- `make lint`
- `make typecheck`
- `make test`
- `make test-e2e`
- `make build`

## 默认接口

- `GET /health`
- `GET /docs`
- `GET /demo`
- `GET /api/v1/site/config`
- `GET /api/v1/site/features`
- `GET /api/v1/site/client-endpoints`
- `POST /api/v1/site/leads`
- `POST /api/v1/auth/login`
- `POST /api/v1/auth/refresh`
- `POST /api/v1/auth/logout`
- `GET /api/v1/users/me`
- `GET /api/v1/site/leads`

## 文档

- [本地开发与整体计划](./docs/backend-local-dev-plan.md)
- [功能演练流程](./docs/feature-walkthrough.md)
- [部署 Runbook](./docs/deployment-runbook.md)
- [环境变量说明](./docs/environment-variables.md)
