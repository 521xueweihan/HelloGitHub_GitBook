# 《HelloGitHub》第 16 期
>兴趣是最好的老师，<a target="\_blank" href="https://hellogithub.com">HelloGitHub</a> 就是帮你找到编程的兴趣！

![](/volume01/img/hello-github.jpg)

---
｜**以下为本期内容**｜每个月 28 号发布最新一期｜<a target="\_blank" href="https://github.com/521xueweihan/HelloGitHub#往期回顾">点击查看往期内容</a>｜

#### C 项目
1、[Tinyhttpd](https://github.com/EZLippi/Tinyhttpd)：一个不到 500 行的超轻量型 HTTP Server，可以用来理解服务器程序的原理和本质。快看 C语言 的入门级项目！

#### C# 项目
2、[VerificationCode](https://github.com/eatage/VerificationCode)：滑动验证码 Demo，示例代码如下：
```javascript
$(function () {
	/******************************************************
	 * 参数一 验证码图片规格 "300*300", "300*200", "200*100"
	 * 参数二 校验通过时执行的函数名
	 * 绑定的div width与图片宽一致 height为图片高加34像素
	 ******************************************************/
	$("#__Verification").slide("200*100", "test");
})
```

![](/volume16/img/VerificationCode.gif)

3、[WeixinSDK](https://github.com/Wlitsoft/WeixinSDK)：微信 C# 版 SDK，虽然现在已经有很多优秀的 SDK，但是本项目的更多的是交流、学习。每个类均有完整的代码注释、对应的单元测试、代码易于理解、接口抽象易于扩展。代码实例如下：

```
using Wlitsoft.Framework.WeixinSDK.Core;
using Wlitsoft.Framework.WeixinSDK.Message.Request.Event;
using Wlitsoft.Framework.WeixinSDK.Message.Response;

namespace WeixinSDK.Test.Fake
{
    /// <summary>
    /// 订阅事件消息 Key_001 请求处理。
    /// </summary>
    public class RequestSubscribeEventMessageKey_001ProcessFake : WeixinMessageProcessBase
    {
        #region WeixinMessageProcessBase 成员

        /// <summary>
        /// 执行处理。
        /// </summary>
        public override void Process()
        {
            RequestSubscribeEventMessage requestMessage = base.GetRequestMessage<RequestSubscribeEventMessage>();

            ResponseTextMessage responseMessage = new ResponseTextMessage()
            {
                Content = requestMessage.EventKey
            };

            base.ResponseMessage = responseMessage;
        }

        #endregion
    }
}
```

#### C++ 项目
4、[vnote](https://github.com/tamlok/vnote)：Markdown 编辑软件。舒适的 Markdown 编辑体验，Vim 操作模式，编辑时代码块高亮

![](/volume16/img/vnote-min.png)

5、[RedisDesktopManager](https://github.com/uglide/RedisDesktopManager)：Redis 桌面管理工具

![](/volume16/img/RedisDesktopManager-min.png)

#### Go 项目
6、[excelize](https://github.com/360EntSecGroup-Skylar/excelize)：操作 XLSX 文件，支持 Microsoft Excel™ 2007 以更高版本

#### Java 项目
7、[SSM](https://github.com/crossoverJie/SSM)：基于现在流行的 `Spring+SpringMVC+Mybatis` 框架，逐步搭建一个现在互联网流行的项目架构。特点：
- 门槛低，**绝对适合新手**
- 从最基本的整合三大框架开始
- 逐步重构为用 `dubbo` 构建微服务
- 其中不乏实际开发中的实战 demo
- 持续更新，已经开始切换到 `SpringBoot+SpringCloud` 构建微服务应用

![](/volume16/img/SSM-min.jpeg)

8、[android-interview-questions-cn](https://github.com/stormzhang/android-interview-questions-cn)：很全面、高质量 Android 面试指南

9、[SmartRefreshLayout](https://github.com/scwang90/SmartRefreshLayout)：强大，稳定，成熟的 Android下 拉刷新框架，集成了各种的炫酷、多样、实用、美观的 Header 和 Footer

![](/volume16/img/SmartRefreshLayout.gif)

#### JavaScript 项目
10、[mvvm](https://github.com/DMQ/mvvm)：剖析 vue 实现原理，了解 vue 的双向数据绑定原理以及核心代码模块，自己动手实现简易版 mvvm

11、[GifW00t](https://github.com/yaronn/GifW00t)：纯 JavaScript 写的 Web 录像插件，可以用来实现网页在线游戏回放、反馈网站 bug、演示用途等，实用举例：
- [Packman 游戏](http://s3-us-west-2.amazonaws.com/anigif100/pacman/index.html)
- [Helicopter 游戏](http://s3-us-west-2.amazonaws.com/anigif100/examples/helicopter/index.html)
- [在线画板](http://s3-us-west-2.amazonaws.com/anigif100/examples/paint/paint.html)

12、[docker-dashboard](https://github.com/pipiliang/docker-dashboard)：基于控制台的 docker 工具，代码简单易读，可以做为学习 Node.js 的实践项目

![](/volume16/img/docker-dashboard-min.png)

13、[APlayer](https://github.com/DIYgod/APlayer)：漂亮的 HTML5 音乐播放器

![](/volume16/img/APlayer-min.png)

14、[DPlayer](https://github.com/DIYgod/DPlayer)：可爱的弹幕视频播放器

![](/volume16/img/DPlayer-min.jpeg)

#### Python 项目
15、[LearnPython](https://github.com/xianhu/LearnPython)：这一个以”撸代码“的形式学习 Python 的编程技巧的项目，针对 Python 的一些语法特性力求通过代码例子解释该知识点、同时还有一些实践项目，通过动手实践有助于知识的融会贯通。同时可以关注作者的[知乎专栏](https://zhuanlan.zhihu.com/pythoner)学习更多的 Python 编程技巧

16、[getproxy](https://github.com/fate0/getproxy)：极简的抓取代理项目，无需配置。不仅提供了获取代理脚本，同时可以通过[该页面](https://github.com/fate0/proxylist/blob/master/proxy.list)，直接获取可用代理（15min 更新、类型包含http和https）

17、[syncPlaylist](https://github.com/Denon/syncPlaylist)：在网易云音乐与 QQ 音乐之间同步歌单。易于使用、配置方便、代码简单，用到的技术：`requests` + `beautifulsoup` 以及 `selenium` + `phantomjs`

18、[GetSubtitles](https://github.com/gyh1621/GetSubtitles)：通过拖曳视频文件进终端，**一步下载字幕** 到视频对应文件夹，并重命名字幕名称为视频名称。Ubuntu 16.04、Windows 10上测试通过，同时兼容 Python2、3。Python 的魅力之一就是可以**快速实现一个适合自己的小工具** Cool ✌️

![](/volume16/img/GetSubtitles.gif)

#### 其它
19、[You-Dont-Need-jQuery](https://github.com/oneuijs/You-Dont-Need-jQuery)：前端发展很快，现代浏览器原生 API 已经足够好用。有些场景下我们并不需要为了操作 DOM、Event 等再学习一下 jQuery 的 API，该项目总结了大部分 jQuery API 替代的方法，[中文](https://github.com/oneuijs/You-Dont-Need-jQuery/blob/master/README.zh-CN.md)

20、[useful-scripts](https://github.com/oldratlee/useful-scripts)：一些平时实用的脚本

21、[restful-api-design-references](https://github.com/aisuhua/restful-api-design-references)：RESTful API 设计参考文献列表，可帮助你更加彻底的了解 REST 风格的接口设计

22、[Bash-Snippets](https://github.com/alexanderepstein/Bash-Snippets)：实用、有趣的 shell 脚本集合

23、[feather](https://github.com/colebemis/feather)：简洁、清爽、免费的 icon 集合

#### 机器学习
24、[ncnn](https://github.com/Tencent/ncnn)：腾讯开源的一个为手机端极致优化的高性能神经网络前向计算框架

25、[tutorials](https://github.com/MorvanZhou/tutorials)：机器学习入门教程，十分详细包含视频教程、文字教程



---

## END
