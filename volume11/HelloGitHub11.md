# 《HelloGitHub》第 11 期
>兴趣是最好的老师，[HelloGitHub](https://github.com/521xueweihan/HelloGitHub) 就是帮你找到兴趣！

![](/volume01/img/hello-github.jpg)

---
｜**以下为本期内容**｜每个月 28 号发布最新一期，首发在我的 [GitHub](https://github.com/521xueweihan) 上｜[点击查看往期内容](https://github.com/521xueweihan/HelloGitHub#往期回顾)｜

#### Python 项目
1、[sh](https://github.com/amoffat/sh)：sh 是一个成熟，用于替代 subprocess，它允许你调用任何程序，就像它是一个函数，支持 Python2.6 - 3.5

```python
from sh import ifconfig
print ifconfig("eth0")
```

2、[fastText.py](https://github.com/salestock/fastText.py)：fastText 简而言之，就是把文档中所有词通过 lookup table 变成向量，取平均后直接用线性分类器得到分类结果。[fastText 的实现](https://www.zybuluo.com/Wayne-Z/note/460881)

3、[mongoaudit](https://github.com/stampery/mongoaudit)：强大的 MongoDB 渗透测试工具，用于发掘 MongoDB 漏洞、并提出改善方法。
- 安装：`pip install mongoaudit`
- 运行：`python mongoaudit`

#### Go 项目
4、[negroni](https://github.com/urfave/negroni)：Negroni 是一个很地道的 Web 中间件，它不是一个框架，是为了方便使用 net/http 而设计的一个库而已。[中文介绍](https://github.com/urfave/negroni/blob/master/translations/README_zh_cn.md)

#### Javascript 项目
5、[react-tetris](https://github.com/chvin/react-tetris)：逼真的俄罗斯方块（非常逼真、强大！），详细的技术介绍，[在线试玩](https://chvin.github.io/react-tetris/?lan=zh)

![](/volume11/img/tetris.gif)

#### Android 项目
6、[WechatLuckyMoney](https://github.com/veryyoung/WechatLuckyMoney)：微信抢红包插件，基于 Xposed 框架，速度快得冷人发指。为避免过度拉仇恨，请谨慎使用（哈哈哈😄）。

![](/volume11/img/wechatluckymoney.gif)

7、[GitClub](https://github.com/TellH/GitClub)：GitClub 不仅仅是一个 GitHub 客户端，还是一个发现优秀 GitHub 开源项目的 App

#### Java 项目
8、[tale](https://github.com/otale/tale)：简洁、漂亮、轻量级、Java 博客，[在线预览](https://tale.biezhi.me/)。特性：
- 设计简洁，界面美观
- Markdown 文章发布
- 自定义文章链接
- 支持多主题
- 支持 Emoji 表情
- 支持网易云音乐播放
- 支持附件和数据库备份
- 部署简单，不依赖 Tomcat

![](/volume11/img/tale-show-min.png)

9、[jvm-mon](https://github.com/ajermakovics/jvm-mon)：命令行模式的 JVM 监控

![](/volume11/img/jvm-show-min.png)

#### C 项目
10、[wrk](https://github.com/wg/wrk)：现代 HTTP 基准测试（实现对一类测试对象的某项性能指标进行定量的和可对比的测试）工具，使用示例：
```sh
# 输入命令
wrk -t12 -c400 -d30s http://127.0.0.1:8080/index.html

# 输出
Running 30s test @ http://127.0.0.1:8080/index.html
  12 threads and 400 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency   635.91us    0.89ms  12.92ms   93.69%
    Req/Sec    56.20k     8.07k   62.00k    86.54%
  22464657 requests in 30.00s, 17.76GB read
Requests/sec: 748868.53
Transfer/sec:    606.33MB
```

#### Swift 项目
11、[Swift30Projects](https://github.com/soapyigu/Swift30Projects)：30 个小型 Swift Apps，可以用来上手学习、练习移动开发。

![](/volume11/img/swift30projects-show-min.jpg)

#### 开源书籍
12、[book](https://github.com/qyuhen/book)：雨痕大神写的学习笔记

13、[nginx-book](https://github.com/taobao/nginx-book)：Nginx 开发从入门到精通——本书的作者为淘宝核心系统服务器平台组的成员

14、[real-world-haskell-cn](https://github.com/huangz1990/real-world-haskell-cn)：《Real World Haskell》中文翻译项目

15、[open-shell-book](https://github.com/tinyclub/open-shell-book)：《Shell 编程范例》，面向操作对象学 Shell！

16、[python-data-structure-cn](https://github.com/facert/python-data-structure-cn)：《Problem Solving with Algorithms and Data Structures using Python》中文版

17、[docker_practice](https://github.com/yeasy/docker_practice)：Dokcer 从入门到实践

18、[explore-flask](https://github.com/rpicard/explore-flask)：[《explore flask》中文翻译](https://spacewander.github.io/explore-flask-zh/index.html)

19、[react-cookbook](https://github.com/shimohq/react-cookbook)：编写简洁漂亮，可维护的 React 应用

20、[rust-book-chinese](https://github.com/KaiserY/rust-book-chinese)：Rust 程序设计语言 中文版

#### 其它
21、[linux-command](https://github.com/jaywcjlove/linux-command)：Linux 命令大全搜索工具，内容包含 Linux 命令手册、详解、学习、搜集

22、[chinese-programmer-wrong-pronunciation](https://github.com/shimohq/chinese-programmer-wrong-pronunciation)：中国程序员容易发音错误的单词

23、[go-lang-cheat-sheet](https://github.com/a8m/go-lang-cheat-sheet)：（英文）Go 语法特性集合

---

## END
