# 《HelloGitHub》第 12 期
>兴趣是最好的老师，[HelloGitHub](https://github.com/521xueweihan/HelloGitHub) 就是帮你找到兴趣！

![](/volume01/img/hello-github.jpg)

---
｜**以下为本期内容**｜每个月 28 号发布最新一期，首发在我的 [GitHub](https://github.com/521xueweihan) 上｜[点击查看往期内容](https://github.com/521xueweihan/HelloGitHub#往期回顾)｜

#### Python 项目
1、[mycli](https://github.com/dbcli/mycli)：mycli 是一个带语法高亮、自动补全的 MySQL 命令行客户端工具。例如，连接数据库方法：`mycli -h localhost -u 用户名 数据库`

![](/volume12/img/mycli.gif)

2、[python-fire](https://github.com/google/python-fire)：Fire 是 Google 开源的 Python 库，可自动将您的代码转变成 CLI，无需您做任何额外工作。您不必定义参数，设置帮助信息，或者编写定义代码运行方式的 main 函数。相反，您只需从 main 模块调用“Fire”函数，其余工作全部交由 Python Fire 来完成。示例代码如下：
```python
import fire
class Example(object):
    def hello(self, name='world'):
        """Says hello to the specified name."""
        return 'Hello {name}!'.format(name=name)

def main():
    fire.Fire(Example)
if __name__ == '__main__':
    main()

# 在终端中调用效果如下：
$ ./example.py hello
Hello world!
$ ./example.py hello David
Hello David!
$ ./example.py hello --name=Google
Hello Google!
```

#### Go 项目
3、[wuzz](https://github.com/asciimoo/wuzz)：wuzz 是用于调试 HTTP 请求的交互式命令行工具，可以用来检查和修改请求。常用操作如下：

| Keybinding | Description |
| :--------- | :------ |
| Ctrl+R | 发送请求 |
| Ctrl+C | 退出 |
| Ctrl+K,Shift+Tab | 前视图 |
| Ctlr+J,Tab | 下一个视图 |
| Ctrl+H,Alt+H | 打开／关闭历史 |
| Down | 向下移动一条视图线 |
| Up | 向上移动一条视图线 |
| Page down | 向下移动一个视图页 |
| Page up | 向下移动一个视图页 |
| F2 | 跳转到 URL |
| F3 | 跳转到查询参数 |
| F4 | 跳转到 HTTP 方法 |
| F5 | 跳转到请求体 |
| F6 | 跳转到 header |
| F7 | 跳转到搜索 |
| F8 | 跳转到响应 header |
| F9 | 跳转到响应体 |

![](/volume12/img/wuzz.gif)

4、[sshtron](https://github.com/zachlatta/sshtron)：sshtron 是通过 SSH 运行的多人贪吃蛇游戏，命令行输入：`ssh sshtron.zachlatta.com`，无需安装等待几秒即可进行游戏（因为服务器在国外，很卡😅）

![](/volume12/img/sshtron.gif)

#### JavaScript 项目
5、[vue2-elm](https://github.com/bailicangdu/vue2-elm)：基于 vue2 + vuex 构建一个大型单页面应用，此项目大大小小共 45 个页面，涉及注册、登录、商品展示、购物车、下单等等，是一个完整的流程，

![](/volume12/img/vue2-elm-show-min.png)

6、[standard](https://github.com/feross/standard)：统一 JavaScript，只需一种样式，[中文](https://github.com/feross/standard/blob/master/docs/README-zhtw.md)

7、[screenfull.js](https://github.com/sindresorhus/screenfull.js)：极小、跨平台的 JavaScript 全屏插件，[在线 demo](https://sindresorhus.com/screenfull.js/)

8、[octotree](https://github.com/buunguyen/octotree)：为 GitHub 和 GitLab 网站，提供直观地显示项目目录结构的浏览器插件，效果如下：

![](/volume12/img/octotree-show-min.png)

#### C# 项目
9、[ScreenToGif](https://github.com/NickeManarin/ScreenToGif)：此工具可以记录屏幕的选定区域、网络摄像头的实时图像和绘图板上的实时图像。可以编辑并将动画保存为 GIF 或视频

![](/volume12/img/screen-to-gif-show-min.png)

#### Android 项目
10、[fresco](https://github.com/facebook/fresco)：Facebook 开源的 Android 管理图片的库，[中文文档](https://www.fresco-cn.org/docs/index.html)。包含功能如下：
- 显示占位图直到加载完成
- 下载图片
- 缓存图片
- 图片不再显示时，从内存中移除
- 等等

#### C 项目
11、[tbox](https://github.com/tboox/tbox)：一个用 C 语言实现的跨平台开发库，用于解决不同操作系统的兼容问题，并且充分利用了各个平台独有的一些特性进行优化。[中文说明](https://github.com/tboox/tbox/blob/master/README_zh.md)


#### Objective-C 项目
12、[bitbar](https://github.com/matryer/bitbar)：Bitbar 是可以将任何（自己或别人写好的）脚本的**输出**到 Mac OS 的状态栏上。同时，支持自定义更新频率。例如：比特币的价格、HelloGitHub 项目的 star 数量（欢迎 star 本项目😄），使用步骤如下：

1. 运行该程序，选择脚本所在目录
2. 确保脚本的有执行权限，赋予执行权限的命令：`chmod +x script.sh`
3. 选择 `Refresh all`，刷新使之生效

![](/volume12/img/bitbar-show-min.png)

#### 开源书籍
13、[explore-python](https://github.com/ethan-funny/explore-python)：感谢 [ethan-funny](https://github.com/ethan-funny) **编写并推荐** 的《Python 之旅》，该书总结了 Python 相关的知识点，力求深入浅出、条理清晰。

14、[The-Art-Of-Programming-By-July](https://github.com/julycoding/The-Art-Of-Programming-By-July/blob/master/ebook/zh/Readme.md)：《编程之法：面试和算法心得》

15、[react-naive-book](https://github.com/huzidaha/react-naive-book)：开源、免费、专业、简单的 React.js 教程

#### 其它
16、[performance-column](https://github.com/barretlee/performance-column)：[阿里胡子哥](https://github.com/barretlee)写的《性能专栏》，旨在提升 PC/H5/Native 等多个端上对性能的认知，[阅读地址](https://github.com/barretlee/performance-column/issues)

17、[node-interview](https://github.com/ElemeFE/node-interview)：如何通过饿了么 Node.js 面试

18、[android-open-project](https://github.com/Trinea/android-open-project)：Android 开源项目集合

19、[gophers](https://github.com/egonelbre/gophers)：Go 吉祥物的各种图片素材

20、[algs4](https://github.com/kevin-wayne/algs4)：（英文）算法第四版书中的示例代码（Java）

---

## END
