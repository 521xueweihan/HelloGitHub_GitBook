# 《HelloGitHub》第 22 期
>兴趣是最好的老师，<a target="\_blank" href="https://hellogithub.com">HelloGitHub</a> 就是帮你找到编程的兴趣！

![](/volume01/img/hello-github.jpg)

---
｜**以下为本期内容**｜每个月 28 号发布最新一期｜<a target="\_blank" href="https://github.com/521xueweihan/HelloGitHub#往期回顾">点击查看往期内容</a>｜

#### C++ 项目
1、[albert](https://github.com/albertlauncher/albert)：Linux 平台下类似于 Mac Alfred 效率神器。支持开机自启动、自定义快捷键等功能

![](/volume22/img/albert-show-min.png)

#### Go 项目
2、[rainbond](https://github.com/goodrain/rainbond)：[好雨](http://www.rainbond.com/)开源的生产级无服务器 PaaS。用于为云原生应用的整个交付流程提供生产级支持，包括基础设施管理、容器化改造、微服务架构转型、DevOps 工作流落地、混合云多云管理等

![](/volume22/img/rainbond-show-min.png)

#### Java 项目
3、[awesome-java-leetcode](https://github.com/Blankj/awesome-java-leetcode)：[LeetCode](https://leetcode.com/) 上面主要收集了各大 IT 公司的笔试面试题。该项目为 LeetCode Java 语言的题解集合

4、[GSYVideoPlayer](https://github.com/CarGuo/GSYVideoPlayer)：Android 视频播放器。支持弹幕、滤镜、水印、截图、边播边缓存、重力旋转与手动旋转的同步等多种功能

![](/volume22/img/GSYVideoPlayer.gif)

5、[FloatWindow](https://github.com/yhaolpz/FloatWindow)：Andorid 任意界面悬浮窗组件，功能丰富，使用简单。特性如下：
- 支持拖动、自动贴边等动画
- 内部自动进行权限申请操作
- 应用退到后台时，悬浮窗会自动隐藏
- 等等

![](/volume22/img/FloatWindow.gif)

6、[anychat](https://github.com/dianbaer/anychat)：纯净的 WebSocket 聊天插件。服务器绝对控制权的推送机制，合理的线程设计，[在线 Demo](https://www.threecss.com/AnyChatClient/third-embed-demo.html)。功能如下：
- 对接任何身份系统
- 个人聊天、群聊天
- 查看聊天记录
- 离线消息推送
- 支持嵌入式，通过 iframe 即可进行嵌入
- 等等

![](/volume22/img/anychat-show-min.png)

#### JavaScript 项目
7、[webpack-component-loader](https://github.com/nicholaslee119/webpack-component-loader)：在不借助框架的情况下，实现 Web component 的标准。该项目对于理解组件化的概念很有帮助

![](/volume22/img/webpack-component-loader-show-min.png)

8、[handsontable](https://github.com/handsontable/handsontable)：强大的开源 HTML5 表格处理工具，适用于中后台的很多业务场景。API 方便、扩展性好、可操作性强，与Execl 等表格处理程序兼容好。并支持非常丰富的操作，如数据绑定、验证、排序及强大的上下文菜单。示例代码如下：
```js
var data = [
  ["", "Tesla", "Volvo", "Toyota", "Honda"],
  ["2017", 10, 11, 12, 13],
  ["2018", 20, 11, 14, 13],
  ["2019", 30, 15, 12, 13]
];

var container = document.getElementById('example');
var hot = new Handsontable(container, {
  data: data,
  rowHeaders: true,
  colHeaders: true,
  filters: true,
  dropdownMenu: true
});
```

9、[learnVue](https://github.com/answershuto/learnVue)：该项目记录了[染陌](https://github.com/answershuto)学习 Vue.js 源码的过程中的心得、收获。以及对于Vue 框架周边库的个人见解。可以帮助开发人员深入地理解 Vue.js 源码

#### Python 项目
10、[shell-functools](https://github.com/sharkdp/shell-functools)：把函数式的编程带入 shell，从而让很多事情变得简单。通过 Python 的高阶函数和内置模块 os.path 与命令的管道结合，达到了强大、高效的功效。相比于单纯的命令实现更加的直观和容易理解，示例代码如下：
```
示例 1
# ls 查看当前目录下的文件
> ls 
document.txt
folder
image.jpg

# 通过 map abspath 展示这些文件的绝对路径
> ls | map abspath
/tmp/demo/document.txt
/tmp/demo/folder
/tmp/demo/image.jpg

示例 2
# find 命令找到的文件和目录
> find
.
./folder
./folder/me.jpg
./folder/subdirectory
./folder/subdirectory/song.mp3
./document.txt
./image.jpg

# 把找到的结果中的文件，重命名在末尾追加 .bak （备份文件）
> find | filter is_file | map basename | map append ".bak"
me.jpg.bak
song.mp3.bak
document.txt.bak
image.jpg.bak
```

11、[tqdm](https://github.com/tqdm/tqdm)：强大、快速、易扩展的 Python 进度条库。我想通过下面的示例代码和效果展示图，你会跑去给这个项目来个 Star 的
```python
from tqdm import tqdm
for i in tqdm(range(10000)):
    pass
# 输出结果：
# 76%|████████████████████████████         | 7568/10000 [00:33<00:10, 229.00it/s]
```

![](/volume22/img/tqdm.gif)

#### 其它
12、[koa-guide](https://github.com/guo-yu/koa-guide)：Node.js Web 框架，Koa 的中文文档

13、[API-Security-Checklist](https://github.com/shieldfy/API-Security-Checklist)：开发安全的 API 所需要核对的清单，[中文](https://github.com/shieldfy/API-Security-Checklist/blob/master/README-zh.md)

14、[http2-explained](https://github.com/bagder/http2-explained)：这是一篇详细讲解 HTTP/2（[RFC 7540](http://httpwg.org/specs/rfc7540.html)）的文档，主要内容包括该协议的背景、思想、协议本身的内容、对一些现有实现的探讨与对协议未来的展望。[中文](https://bagder.gitbooks.io/http2-explained/zh/)

15、[document-style-guide](https://github.com/ruanyf/document-style-guide)：《中文技术文档的写作规范》



---

## END
