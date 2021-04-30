
Windows下搭建环境：

```shell
C:\Python37\python.exe -m venv venv
```

激活python虚拟环境并

```shell
.\venv\Scripts\Activate.ps1
```

```shell
pip list
```

```shell
Package    Version
---------- -------
pip        10.0.1
setuptools 39.0.1
You are using pip version 10.0.1, however version 21.1 is available.
You should consider upgrading via the 'python -m pip install --upgrade pip' command.
```

升级pip：

```shell
python -m pip install --upgrade pip -i https://pypi.douban.com/simple/
```

升级成功：

```shell
Package    Version
---------- -------
pip        21.1
setuptools 39.0.1
```

安装依赖：

```shell
python -m pip install -r requirements.txt -i https://pypi.douban.com/simple/
```

安装成功后：

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

初始化目录及设置

```shell
sphinx-quickstart
```

```shell
Welcome to the Sphinx 3.5.4 quickstart utility.

Please enter values for the following settings (just press Enter to
accept a default value, if one is given in brackets).

Selected root path: .

You have two options for placing the build directory for Sphinx output.
Either, you use a directory "_build" within the root path, or you separate
"source" and "build" directories within the root path.
> Separate source and build directories (y/n) [n]:y
```


```shell
The project name will occur in several places in the built documentation.
> Project name: GnuCash-Guide-zh-CN
> Author name(s): zhengmingpei
> Project release []: 

If the documents are to be written in a language other than English,
you can select a language here by its language code. Sphinx will then
translate text that it generates into that language.

For a list of supported codes, see
https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-language.
> Project language [en]:zh_CN
```

输出
```shell
Creating file C:\Users\zheng\Documents\codes2020\gnucash-guide-zh-CN\source\conf.py.
Creating file C:\Users\zheng\Documents\codes2020\gnucash-guide-zh-CN\source\index.rst.
Creating file C:\Users\zheng\Documents\codes2020\gnucash-guide-zh-CN\Makefile.
Creating file C:\Users\zheng\Documents\codes2020\gnucash-guide-zh-CN\make.bat.

Finished: An initial directory structure has been created.

You should now populate your master file C:\Users\zheng\Documents\codes2020\gnucash-guide-zh-CN\source\index.rst and create other documentation
source files. Use the Makefile to build the docs, like so:
   make builder
where "builder" is one of the supported builders, e.g. html, latex or linkcheck.
```

```shell
Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----         2021/4/30     19:47                .vscode # vscode生成的配置文件夹
d-----         2021/4/30     20:16                build # sphinx生成的html输出目录
d-----         2021/4/30     20:16                source # sphinx生成的rst源文档目录
d-----         2021/4/30     20:18                temp # 自己单独添加的临时目录
d-----         2021/4/30     19:58                venv # 自己生成的虚拟python环境目录
-a----         2021/4/30     20:18             19 .gitignore # 源码版本控制文件
-a----         2021/4/30     20:16            799 make.bat # sphinx生成的批处理文件
-a----         2021/4/30     20:16            638 Makefile # sphinx生成的文件
-a----         2021/4/30     20:18           3658 readme.md # 自己编写的说明文档
-a----         2021/4/30     19:56              6 requirements.txt # python环境配置文件
```
