# 某东登录面板

### 配置文件说明

| 字段          | 说明                               | 示例                   |
| ------------- | ---------------------------------- | ---------------------- |
| web_port      | 面板端口                           | 8080                   |
| hostname      | 青龙地址                           | http://baidu.com:8080/ |
| client_id     | 青龙key                            | 123                    |
| client_secret | 青龙secret                         | 123                    |
| disabled      | 是否禁用`true:禁用，false：不禁用` |                        |
| carmi         | 卡密                               |                        |

### 使用说明

#### 一键Docker部署命令
```shell
docker run -itd --name jdWeb -p 3000:3000 -v $PWD/jdWeb:/root/jdWeb --restart=unless-stopped pingxingsheng/jdweb
```

**务必将本仓库的login文件夹复制到用户目录下的jdWeb文件夹下。否测没有界面**

#### docker升级命令

```shell
docker run --rm -v/var/run/docker.sock:/var/run/docker.sock containrrr/watchtower --run-once jdWeb
```

#### 自定义登录界面

将本仓库的login文件夹复制到用户目录下的jdWeb文件夹下，里面的样式和文件都可以自己修改

**注意📢** **注意📢** **注意📢**

**务必将本仓库的login文件夹复制到用户目录下的jdWeb文件夹下。否测没有界面**

启动失败是因为没有正确配置config.json文件，config.json文件位置在用户目录下的jdWeb文件夹下，配置后重新启动容器即可。

### 最后

防止失联，进https://t.me/tigerorrose

## 免责声明

请勿将本仓库内的任何内容用于商业或非法目的，否则后果自负.

如果任何单位或个人认为该项目的脚本可能涉嫌侵犯其权利，则应及时通知并提供身份证明，所有权证明，我将在收到认证文件后删除相关脚本.

作者对任何本仓库中包含的脚本在使用中可能出现的问题概不负责，包括但不限于由任何脚本错误导致的任何损失或损害.

您必须在下载后的24小时内从计算机或手机中完全删除以上内容.

任何以任何方式查看此项目的人或直接或间接使用该项目的任何脚本的使用者都应仔细阅读此声明。作者保留随时更改或补充此免责声明的权利。一旦使用并复制了任何本仓库相关脚本或其他内容，则视为您已接受此免责声明.

### 本仓库之中所有脚本配置纯属自用备份
