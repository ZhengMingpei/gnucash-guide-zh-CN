# gnucash-guide-zh-CN

**最后更新于2021年5月6日。**

本项目为GnuCash的简体中文文档项目，文档由GnuCash的中文使用者(下称**文档编辑者**)对官方英文文档进行本地化、简化和整理制作而成，文档内容仅供参考。

文档内容所有权由原GnuCash文档制作组及本文档编辑者(见末尾)拥有。

## 一、项目介绍

### （一）项目发起原因

我认为，官方文档项目存在以下几个痛点：

* 官方文档内容非常繁多，几百页的文档，对非英语的GnuCash使用者不太友好。
* 通过测试，官方文档项目相对容易在linux下编译成功，但是在windows下有很多比较难处理的依赖，或者说解决起来很麻烦，导致项目参与比较困难。
* 通过测试，官方文档项目中，简单配置编译后，仍旧存在很多中文字符格式错误的问题，比如句段间距不正常、章节标题不正常、字体等。

为了解决上述问题，帮助更多中文用户更轻松地入门GnuCash，帮助更多中文用户更轻松地入门GnuCash，我暂时使用Sphinx制作了在线中文文档，可供参考。

### （二）内容完善及沟通

本文档的结构借鉴官方的GnuCash-Guide文档，内容尚在完善中，欢迎感兴趣的朋友参与文档的编辑、意见反馈、Q&A等，所有参与者将列于**文档编辑者**中。

建有QQ群，名为“gnucash使用交流群”，群号为526047677，欢迎加群了解有关细节。

## 二、通过github参与文档项目

本文档项目借鉴[manim.wiki](https://manim.wiki/)的构建方式，使用`sphinx + github actions`自动构建，构建步骤见下面的内容。

文档编辑需要使用`reStructuredText`标记语言，具体语法见[Sphinx文档](https://zh-sphinx-doc.readthedocs.io/en/latest/rest.html)。

建议参与者使用github账户，采取以下两种编辑文档的方式：

### （一）仅编辑reStructuredText文档

直接Fork项目到自己的账户下，下载后在`master`分支下，使用任意文本编辑器进行`reStructuredText`文档的编辑，最后提交`Pull Request`。

该方式无法预览在线效果。

### （二）编辑并构建html在线文档

Windows下搭建构建环境：

1. 安装python(比如3.7版本到默认目录)

2. 将本项目下载到电脑上某目录(比如gnucash-guide-zh-CN)下，在该目录下创建虚拟python环境

```shell
cd gnucash-guide-zh-CN
C:\Python37\python.exe -m venv venv
```

3. 激活python虚拟环境并安装依赖

```shell
.\venv\Scripts\Activate.ps1
```

> 查看包列表 

```shell
pip list
```

> 没有安装任何包的默认输出：

```shell
Package    Version
---------- -------
pip        10.0.1
setuptools 39.0.1
You are using pip version 10.0.1, however version 21.1 is available.
You should consider upgrading via the 'python -m pip install --upgrade pip' command.
```

> 升级pip：

```shell
python -m pip install --upgrade pip -i https://pypi.douban.com/simple/
```

> 安装依赖：

```shell
python -m pip install -r requirements.txt -i https://pypi.douban.com/simple/
```

> 安装成功后的包列表：

```shell
Package                       Version
----------------------------- ---------
alabaster                     0.7.12
Babel                         2.9.1
certifi                       2020.12.5
chardet                       4.0.0
colorama                      0.4.4
docutils                      0.16
idna                          2.10
imagesize                     1.2.0
Jinja2                        2.11.3
MarkupSafe                    1.1.1
packaging                     20.9
pip                           21.1
Pygments                      2.8.1
pyparsing                     2.4.7
pytz                          2021.1
requests                      2.25.1
setuptools                    39.0.1
snowballstemmer               2.1.0
Sphinx                        3.5.4
sphinxcontrib-applehelp       1.0.2
sphinxcontrib-devhelp         1.0.2
sphinxcontrib-htmlhelp        1.0.3
sphinxcontrib-jsmath          1.0.1
sphinxcontrib-qthelp          1.0.3
sphinxcontrib-serializinghtml 1.1.4
urllib3                       1.26.4
```

以上搭建完毕后，进入`master`分支的`source`目录下，用vscode打开`conf.py`，选择虚拟环境，在打开`index.rst`时,根据提示安装好vscode的`reStructuredText`插件，进行预览，选择`sphinx`即可预览成功。

编辑部分同上。

## 三、文档编辑者

当前编辑者列表：

* zhengmingpei (B站id：yueyawanbian; [B站主页](https://space.bilibili.com/32918983); QQ:1824139500; email: 1824139500@qq.com)
