# 书籍 & 博客文章
接下来一段时间，整理一些自己感兴趣的电子书

# 安装依赖

项目依赖rust一个工具[mdBook](https://rust-lang.github.io/mdBook/)，安装完成后直接在根目录启动服务。
```
mdbook serve -怕 9009
```
正常启动如下所示：
```
2024-06-20 11:30:24 [INFO] (mdbook::book): Book building has started
2024-06-20 11:30:24 [INFO] (mdbook::book): Running the html backend
2024-06-20 11:30:24 [INFO] (mdbook::cmd::serve): Serving on: http://localhost:3000
2024-06-20 11:30:24 [INFO] (mdbook::cmd::watch): Listening for changes...
2024-06-20 11:30:24 [INFO] (warp::server): Server::run; addr=[::1]:3000
2024-06-20 11:30:24 [INFO] (warp::server): listening on http://[::1]:3000
```
启动成功后在浏览器输入 [http://localhost:3000](http://localhost:3000) 。

# 编译
```
mdbook build 计算思维 -d dist
```