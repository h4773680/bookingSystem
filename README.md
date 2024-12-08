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
