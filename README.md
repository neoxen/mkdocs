# mkdocs 使用

## 安装 MkDocs

运行以下命令从命令行安装 MkDocs：

> pip install mkdocs

## 创建新的项目

运行以下命令创建一个新的项目：

> mkdocs new my-project
> cd my-project

## 初始文档结构

``` text
mkdocs.yml    # 配置文件。
docs/
    index.md  # 文档主页。
    ...       # 其他 Markdown 页面、图片和其他文件。
```

## 启动本地服务器

运行以下命令启动本地服务器：

> $ mkdocs serve
> INFO    -  Building documentation...
> INFO    -  Cleaning site directory
> INFO    -  Documentation built in 0.22 seconds
> INFO    -  [15:50:43] Watching paths for changes: 'docs', 'mkdocs.yml'
> INFO    -  [15:50:43] Serving on <http://127.0.0.1:8000/>

用游览器打开 <http://127.0.0.1:8000/> 就可以查看文档了。

## 构建网站

运行以下命令构建网站：

> mkdocs build

## 部署

构建的网站只包含静态文件，所以你可以从任何地方托管它。只需将整个 site 目录的内容上传到你托管网站的位置即可。有关特定主机的详细信息，请参阅部署您的文档页面。

## 其他命令和选项

有各种其他命令和选项可用。要查看完整的命令列表，请使用 --help 标志：

> mkdocs --help

要查看给定命令的所有选项，请使用 --help 标志与该命令。例如，要查看 build 命令的所有选项，请运行以下命令：

> mkdocs build --help

## 源码管理

如果使用源代码管理工具（例如 git），则可能不希望将构建的文档签入到仓库中。在 .gitignore 文件中添加一行 site/ 即可。

> echo "site/" >>.gitignore

如果您使用的是另一个源代码管理工具，请查看其文档以了解如何忽略特定目录。
