# Laravel on Docker

希望成为一个好用的Laravel 的Docker开发环境，取代Homestead，享受容器技术带来的便利。

### 包含的容器

- **数据库**
    - MySQL
    - PostgreSQL
- **数据库管理**
    - phpmyadmin
    - pgadmin
- **全文搜索引擎**
    - Elasticsearch
- **消息队列**
    - RabbitMQ    
- **缓存**
    - Redis
- **WEB服务器**
    - Nginx
- **PHP-FPM**
    - PHP-FPM
- **Workspace**
    - PHP CLI
    - Composer
    - NVM
    - Node.js(6.1.0)
    - Git
    - cURL

### 使用方法

0x1:
- `git clone https://github.com/starriv/laravel-docker.git`

0x2:
- 自行查阅需要运行的容器的Dockerfile及编排(默认为开发环境，线上务必自行修改为安全的方式)

0x3
- `docker-compose build | up {containername}`

### 致谢
[laradock](https://github.com/LaraDock/laradock)
