# 酷狗 · MyGo Music 插件

在 MyGo Music 中搜索、浏览和播放酷狗音乐。插件直接调用酷狗接口。

## 安装和使用

1. 在 MyGo Music 打开 **设置 → 插件 → +**。
2. 选择 **从 GitHub 安装**，输入 `fcmfcm1999/mygo-music-kugou`；或者从该仓库的 Releases 下载 ZIP，再选择 **从本地安装** 并打开 ZIP。
3. 安装时允许插件申请的网络权限，然后在来源选择器中切换到 **酷狗概念版**。
4. 若要查看自己的歌单，点击侧栏底部的账户入口，用酷狗 App 扫描二维码登录。每日推荐和推荐歌单无需登录。

## 功能

- 首页每日推荐和推荐歌单，歌曲显示专辑封面。
- 按歌曲、专辑、歌手或歌单搜索。
- 热门歌手列表、歌手详情和专辑详情。
- 登录酷狗账号、查看个人歌单及歌单曲目。
- 播放歌曲，并获取 LRC 歌词。

侧栏提供首页、每日推荐和歌手入口。推荐歌单仍显示在首页

## 权限和限制

插件需要访问以下酷狗服务：

- `gateway.kugou.com`、`openapi.kugou.com`：歌曲、歌手、专辑、歌单等音乐数据。
- `login-user.kugou.com`：二维码登录。
- `lyrics.kugou.com`、`krcs.kugou.com`：歌词搜索和下载。
- `expendablekmr.kugou.com`：补充歌曲封面。

登录令牌保存在 MyGo Music 的插件数据中；插件不读取酷狗客户端 Cookie。酷狗可能要求部分歌曲先完成设备验证，当前插件无法处理这类验证，因此这些歌曲可能无法播放。音质和可播放范围也会受到酷狗账号权限、歌曲版权及地区限制影响。

## 参考

酷狗接口参数、签名和歌词接口参考 [MakcRe/KuGouMusicApi](https://github.com/MakcRe/KuGouMusicApi)。相关 MIT 许可见本目录 [LICENSE](LICENSE)。
