電影預訂系統
=============
這是一個基於 Flask 的電影預訂系統，允許用戶註冊、登錄、查看電影、預訂座位和管理預訂。系統使用 PostgreSQL 作為數據庫，並利用 Docker 和 Docker Compose 進行容器化部署。

功能
-------------
* 用戶註冊和登錄
* 查看電影列表及詳細信息
* 預訂座位
* 管理預訂（查看和取消預訂）
* JWT 認證

技術
-------------  
* 後端框架：Flask
* 數據庫：PostgreSQL
* ORM：SQLAlchemy
* 身份驗證：Flask-JWT-Extended
* 容器化：Docker 和 Docker Compose

使用方式
------------- 
1. 訪問 `http://localhost:5001` 來使用應用程序。
2. 使用 POST 請求到 `/register` 來註冊新用戶，請求體應包含 `username`、`email` 和 `password`。
3. 使用 POST 請求到 `/login` 來登錄，請求體應包含 `username` 和 `password`，成功登錄後將返回 JWT 令牌。
4. 使用 JWT 令牌訪問受保護的路由，例如預位和查詢電影。
