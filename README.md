# 6盘小白羊 第二版

开饭中，最新2.2.0版全部开源代码已上传  

[12月17日21点45  v2.2.1  https://wws.lanzous.com/b01npsg8h](https://wws.lanzous.com/b01npsg8h)  仅供尝鲜,此版本不兼容旧版数据

[11月8日 v2.1.1 https://wws.lanzous.com/b01nqc4gd](https://wws.lanzous.com/b01nqc4gd)  旧版链接备用

win、linux、mac 均已发布，再接下来要整RSS订阅功能，这是个大项目了。。。。  

#### 2020/12/19
```
1. Fix 重复启动时没有显示当前实例窗口的 BUG
2. Fix 使用 cookie 登录时小写 cookie 提示格式错误的 BUG
3. Fix 下载/上传页面,列表刷新时自动滚动到顶部的 BUG
4. Add 清除所有离线任务时二次确认提示
5. Add 批量导出离线链接按钮
6. Add 批量下载按钮
7. Add 批量改名增加前缀功能
8. Add 提交离线链接支持自动转换迅雷链接格式(thunder://)
```
### 功能介绍

6盘官方网页版功能已基本覆盖。下面是小白羊第二版特色功能<br />

``` diff
+ [√] 多账号同时登录管理
+ [√] 目录树快捷导航(右键菜单:下载文件夹，复制移动，删除到回收站)
+ [√] 在线预览功能（在线预览图片，在线预览文本，在线预览PDF，Doc等），在线播放视频
+ [√] 文件、文件夹批量重命名，批量删除，批量移动
+ [√] 支持一键下载整个文件夹，支持下载队列，多文件同时下载
+ [√] 支持一键上传整个文件夹，支持上传队列，多文件同时上传，支持秒传
+ [√] 文件下载支持断点续传，可以下载超大文件
+ [√] 文件下载完支持自动执行脚本文件回调（参照aria2）
+ [√] 支持通过在浏览器输入IP，远程管理操作
- [ ] RSS订阅功能开发中：~~订阅资源秒传~~
```

### 安装说明

##### 1. Windows  
下载 `6盘小白羊版win64.7z` 解压缩，双击运行 `6盘小白羊版.exe` 即可<br />
已内置mpv播放器可以直接在线预览视频<br />
windows10可能会遇到Defender报毒，需要将小白羊的文件夹添加到排除里，参阅：<br />
 https://blog.csdn.net/qq_43453731/article/details/104722165
##### 2. Mac os  
下载 `6盘小白羊版mac64.7z` 解压缩，双击运行 `6盘小白羊版.app` 即可<br />
已内置mpv播放器可以直接在线预览视频
##### 3. Linux  
下载 `6盘小白羊版linux64.7z` 解压缩，修改 `6盘小白羊版` 这个文件的权限为可执行，然后双击运行即可<br />
linux需要自己安装一次mpv播放器，才可以视频在线预览<br />
打开终端，输入命令  <code>sudo apt-get install mpv -y</code>  安装mpv
<br /><br />
注1：mac如果提示启动被阻止，需要在‘系统偏好设置’--‘安全性与隐私’--‘允许从以下位置下载的App’--‘仍要打开’<br />
注2：mac有时会遇到由于程序未签名导致的白屏（6panserver这个文件没正常运行），此问题我还在研究怎么解决<br />

![https://ae03.alicdn.com/kf/Hcf945f61f47741ec847814d8ec05b9d56.jpg](https://ae03.alicdn.com/kf/Hcf945f61f47741ec847814d8ec05b9d56.jpg)
<br /><br />
[运行截图 点击查看 https://ae03.alicdn.com/kf/Hcf945f61f47741ec847814d8ec05b9d56.jpg](https://ae03.alicdn.com/kf/Hcf945f61f47741ec847814d8ec05b9d56.jpg)
<br />

### 版本升级说明

小白羊无需安装，解压后即可使用，升级新版本时，使用新版文件替换旧版文件即可。目录说明：<br />
```
/6盘小白羊版.exe                        启动程序  
/electron/resources/6panserver.exe     6盘服务程序   
/electron/resources/AppData/www.db     html资源  
/electron/resources/AppData/user.db    *用户数据，第一次启动后创建  
/electron/resources/AppData/debug.log  *运行日志，第一次启动后创建  
...其他文件
```
重点只有这/electron/resources/AppData/user.db文件，里面是用户自己的数据。版本升级时要保留，不要删除  


### 版权声明

6盘小白羊版仅是完全免费的个人学习作品，和6盘官方无任何关联。所有功能均基于调用6盘官方开放API，再此感谢6盘的无私<br /><br />
1.6盘(6pan.cn)是一个网盘，其付费用户每天可以离线下载100个任务（电驴、磁力、BT、百度分享链接）<br />
2.小白羊版只是美化UI，你离线是保存到6盘下载文件是从6盘下，所有服务、内容均由6盘提供请正确认知<br />
3.小白羊版和6盘官方无任何关联，由我个人开发，不能代表6盘官方，但会长期维护<br />
