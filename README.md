# xssblind
- 最近测试ezXSS，最初使用dmap安装，发现特别麻烦，而且各种报错。
- 为了方便，自己尝试做成了docker，需要docker-compose，请提前安装。
- 本项目可以实现一键搭建ezXSS环境，操作方法如下：

## 0x01 快速部署

```bash
git clone https://github.com/hack2012/xssblind.git
cd xssblind
docker-compose build
docker-compose up -d
```

然后访问你的80端口，即可开启安装向导。

## 0x02 管理数据库
访问你的8080端口即可 http://your-ip:8080
- 默认用户名：root
- 默认密码：waitalone.cn

要修改密码，请在`docker-compose.yml`中修改，同时需要修改`www/src/Database.php`中密码

## 0x03 其它问题
1. 若无法生成截图，请修改asserts/img目录权限为777

