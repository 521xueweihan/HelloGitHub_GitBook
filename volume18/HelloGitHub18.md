# 《HelloGitHub》第 18 期
>兴趣是最好的老师，<a target="\_blank" href="https://hellogithub.com">HelloGitHub</a> 就是帮你找到编程的兴趣！

![](/volume01/img/hello-github.jpg)

---
｜**以下为本期内容**｜每个月 28 号发布最新一期｜<a target="\_blank" href="https://github.com/521xueweihan/HelloGitHub#往期回顾">点击查看往期内容</a>｜

#### C 项目
1、[db_tutorial](https://github.com/cstack/db_tutorial)：用 C 从零创建一个简单的数据库

#### CSS 项目
2、[materialize](https://github.com/Dogfalo/materialize)：基于 Material Design 的现代响应式前端框架，简化了前端的开发，文档丰富。[官网](http://materializecss.com/)

#### Go 项目
3、[tidb](https://github.com/pingcap/tidb)：开源分布式 NewSQL 数据库，能优雅的替换传统的数据库中间件、数据库分库分表等 Sharding 方案。具备如下核心特性：
- SQL支持 （TiDB 是 MySQL 兼容的）
- 水平线性弹性扩展
- 分布式事务
- 跨数据中心数据强一致性保证
- 故障自恢复的高可用

![](/volume18/img/tidb-show-min.png)

4、[echo](https://github.com/labstack/echo)：Go 语言最受欢迎的 Web 框架之一，具有：高性能、便于扩展、轻量的特点，示例代码：
```go
package main

import "github.com/labstack/echo"

func main() {
	e := echo.New()
	e.GET("/", callback)
	e.Logger.Fatal(e.Start(":3000"))
}

func callback(ctx echo.Context) error {
	return ctx.HTML(200, "<h1>你好 echo</h1>")
}
```

![](/volume18/img/echo-show-min.png)

#### Java 项目
5、[AndroidTVLauncher](https://github.com/JackyAndroid/AndroidTVLauncher)：一个 TV Leanback 风格桌面，基于 Leanback 库开发，符合 Android TV 官方交互规范

![](/volume18/img/AndroidTVLauncher-show-min.png)

6、[spring-data-jpa-datatables](https://github.com/darrachequesne/spring-data-jpa-datatables)：spring-data-jpa 和 jQuery [datatables](https://www.datatables.net/) 集成工具。极大简化基于 datatables 数据表格的开发，示例代码：
```
// 前端代码
$(document).ready(function() {
	var table = $('table#sample').DataTable({
		'ajax': {
			'contentType': 'application/json',
			'url': '/data/users',
			'type': 'POST',
			'data': function(d) {
				return JSON.stringify(d);
			}
		},

// java 代码 server-side becomes
@JsonView(DataTablesOutput.View.class)
@RequestMapping(value = "/data/users", method = RequestMethod.POST)
public DataTablesOutput<User> getUsers(@Valid @RequestBody DataTablesInput input) {
	return userRepository.findAll(input);
}
```

![](/volume18/img/spring-data-jpa-datatables-show-min.png)

7、[xxl-job](https://github.com/xuxueli/xxl-job)：轻量级分布式任务调度框架，其核心设计目标是：开发迅速、学习简单、轻量级、易扩展，文档齐全。[官网](http://www.xuxueli.com/xxl-job/)

#### JavaScript 项目
8、[flatpickr](https://github.com/chmln/flatpickr)：扁平化的日期选择组件，项目源码使用 TypeScript 编写，可以学习使用 Typescript 编写 JS 插件，Typescript 语言的好处是：可以在多人协作中避免一些变量类型错误的问题，从而提高效率。使用示例代码：
```javascript
// ConnonJS 方式引入
const flatpickr = require("flatpickr");
flatpickr("#myID", {});
flatpickr(".myClass", {});

// jQuery 方式引入
$(".selector").flatpickr(optional_config);
```

![](/volume18/img/flatpickr-show-min.png)

9、[vue-3d-model](https://github.com/hujiulong/vue-3d-model)：展示三维模型的 Vue 组件，支持模型操作和模型点击事件，能自动缩放模型到合适大小并校正偏移，目前支持 obj、stl、dae 和 json 格式的模型，示例代码：
```vue
<template>
    <model-obj src="example/models/obj/LeePerrySmith.obj"></model-obj>
</template>
<script>
    import { ModelObj } from 'vue-3d-model'

    export default {
        components: { ModelObj }
    }
</script>
```

![](/volume18/img/vue-3d-model.gif)

10、[weweChat](https://github.com/trazyn/weweChat)：微信的第三方客户端。在完整实现 Web 微信功能的基础上，新增并优化部分功能，重设计整体 UI，提供更好的体验。Mac 安装命令：`brew cask install wewechat`

![](/volume18/img/weweChat-show-min.png)

11、[puppeteer](https://github.com/GoogleChrome/puppeteer)：Google Chrome 团队开源的面向 Node.js 的，基于 DevTools 协议的远程 Headless Chrome 控制库，它可以生成网页截图、PDF、抓取单页应用与网页内容、进行自动化表单提交、界面测试与模拟键盘输入等功能。示例代码如下：
```javascript
// 访问 https://example.com 并将截图保存为 example.png
const puppeteer = require('puppeteer');

(async () => {
  const browser = await puppeteer.launch();
  const page = await browser.newPage();
  await page.goto('https://example.com');
  await page.screenshot({path: 'example.png'});

  await browser.close();
})();
```

12、[SelectPage](https://github.com/TerryZ/SelectPage)：简洁优雅而功能强大的选择器，使用简单，适应各种UI环境，功能强大，丰富的参数和回调函数
。它包含了 autocomplete、ajax 数据源、多选择 Tag、i18n 国际化，结果列表分页展示，键盘快捷操作等
```javascript
//defined a array, the data returned at the server side is also used that format：
//Array[{Object},{...}]
var data = [
    {id:1 ,name:'Chicago Bulls',desc:'芝加哥公牛'},
    {id:2 ,name:'Cleveland Cavaliers',desc:'克里夫兰骑士'},
    {id:3 ,name:'Detroit Pistons',desc:'底特律活塞'},
    {id:4 ,name:'Indiana Pacers',desc:'印第安纳步行者'}
];
//init SelectPage
$('#selectpage').selectPage({
    showField : 'desc',
    keyField : 'id',
    data : data
});
```

![](/volume18/img/SelectPage-show-min.png)

#### PHP 项目
13、[wooyun_public](https://github.com/hanc00l/wooyun_public)：乌云公开漏洞、知识库爬虫和搜索

![](/volume18/img/wooyun-show-min.png)

#### Python 项目
14、[pygorithm](https://github.com/OmkarPathak/pygorithm)：一个帮助学习主要算法的库，可以通过理解这些算法的实现，提高自己的算法水平。冒泡排序示例：
```python
>>> from pygorithm.sorting import bubble_sort
>>> my_list = [12, 4, 3, 5, 13, 1, 17, 19, 15]
>>> sorted_list = bubble_sort.sort(my_list)
>>> print(sorted_list)
>>> [1, 3, 4, 5, 12, 13, 15, 17, 19]
```

15、[newspaper](https://github.com/codelucas/newspaper)：强大的提取 Web 的内容、文章的库，支持多种语言，安装命令 `pip3 install newspaper3k`。示例代码：
```python
>>> from newspaper import Article

>>> url = 'http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-pot-guns-and-drones/'
>>> article = Article(url)

>>> article.download()

>>> article.html
'<!DOCTYPE HTML><html itemscope itemtype="http://...'

>>> article.parse()

>>> article.authors
['Leigh Ann Caldwell', 'John Honway']

>>> article.publish_date
datetime.datetime(2013, 12, 30, 0, 0)

>>> article.text
'Washington (CNN) -- Not everyone subscribes to a New Year's resolution...'

>>> article.top_image
'http://someCDN.com/blah/blah/blah/file.png'

>>> article.movies
['http://youtube.com/path/to/link.com', ...]

>>> from newspaper import Article
>>> url = 'http://www.bbc.co.uk/zhongwen/simp/chinese_news/2012/12/121210_hongkong_politics.shtml'

>>> a = Article(url, language='zh') # Chinese

>>> a.download()
>>> a.parse()

>>> print(a.text[:150])
香港行政长官梁振英在各方压力下就其大宅的违章建
筑（僭建）问题到立法会接受质询，并向香港民众道歉。
梁振英在星期二（12月10日）的答问大会开始之际
在其演说中道歉，但强调他在违章建筑问题上没有隐瞒的
意图和动机。 一些亲北京阵营议员欢迎梁振英道歉，
且认为应能获得香港民众接受，但这些议员也质问梁振英有

>>> print(a.title)
港特首梁振英就住宅违建事件道歉
```

16、[faker](https://github.com/joke2k/faker)：用于生成假数据的库，支持多种语言，你值得拥有。示例代码：
```python
fake.address()
# '辽宁省雪市静安廉街b座 998259'

fake.street_address()
# '巢湖街U座'

fake.building_number()
# 'x座'

fake.city_suffix()
# '市'

fake.latitude()
# Decimal('-0.295126')

fake.province()
# '湖北省'
```

#### 其它
17、[ctf-wiki](https://github.com/ctf-wiki/ctf-wiki)：一个自由的站点，主要包含了 CTF 的基础知识 、常见题型、解题思路以及常用工具等，希望可以帮助你更快地了解 CTF 竞赛以及网络安全相关知识

18、[china_area_mysql](https://github.com/kakuilan/china_area_mysql)：中国 5 级行政区域 MySQL 库

19、[open_source_team](https://github.com/niezhiyang/open_source_team)：国内顶尖团队的开源地址

#### 机器学习
20、[deeplearningbook-chinese](https://github.com/exacity/deeplearningbook-chinese)：Deep Learning 中文版



---

## END
