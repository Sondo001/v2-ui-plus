# Owner: Dự án gốc nằm ở đây [**Nick-Hopps**](https://github.com/Nick-Hopps/v2-ui-plus) tôi chỉ phát triển lại nó

# V2 X-UI Unofficial
```
Đây Là Phiên Bản X-UI được Việt Hoá và cập nhật Xray định kỳ.
```

# 注意

这是 [v2-ui](https://github.com/sprov065/v2-ui) 原作者版本的加强版，增加账号管理、单端口多用户等功能，更多功能还在二次开发中。

另外当前项目内的脚本 `install.sh` 还没有更改，因此推荐暂时使用 `python v2-ui.py` 运行本项目。同时因为还处于开发中，因此还不打算出静态编译的版本，有需要的可以自行编译。

# 已完成的功能

- `修复` 修复已有的 BUG 并优化部分功能；
- `新增` 增加账号管理功能
  - 可添加普通用户和管理员用户，默认第一个用户为管理员用户且无法删除；
  - 可批量启动/关闭/删除多个账号，且可按创建/用户名/流量递增递减排序；
  - 每个用户可独立添加多个入站配置，每个入站配置单独统计流量。
- `特性` 现在已经可以添加相同端口的配置，写入配置文件前自动合并相同协议相同端口的配置；
- `优化` 修改流量统计方式为 “email”，方便配置合并后独立统计各个入站配置的流量;
- `新增` 增加 Dockerfile，自行编译后即可在 Docker 中使用本项目；
- `新增` 增加 “v2ray 外部端口” 设置项，显示 Haproxy 或者 Nginx 代理时的外部端口从而生成正确的配置链接/二维码；
- `新增` 增加 “v2ray 外部 TLS” 设置项，显示 Haproxy 或者 Nginx 代理时的 TLS 状态从而生成正确的配置链接/二维码；
- `修复` 修复日志功能，现在日志可以成功输出到 stdout 和日志文件；
- `新增` 增加 “使用 Xray-Core” 设置项，可替换 Core 为 Xray-Core，并增加 fallback 支持；
- `新增` 使用修饰器简单实现鉴权功能；
- `修复` 现在 “按创造顺序” 排序可以正常使用了。

# 正在开发中的功能

暂无

# 计划增加的功能

- 可以使用 Nginx/Caddy 等 HTTP 服务器代替 Tornado；

# 目前存在的问题

- 用户界面配置不齐全。

# 界面展示

![screenshot_1.png](screenshot_1.png)

![screenshot_2.png](screenshot_2.png)
