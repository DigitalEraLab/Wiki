# 纪元数位Wiki

本项目用于搭建纪元数位公司的wiki网站。

## 文件结构说明

以下是整个项目结构：

```
├── docs
│   ├── index.md
│   ├── Sovits+vits
│   ├── Stable-diffusion_lora
│   │   └── README.md
│   └── Wav2lip+GFPGAN
├── mkdocs.yml
└── ReadME.md
```

`docs`是放说明文档的文件夹，Sovits+vits等是子目录，该wiki网站通过多级目录实现多级导航。

 `mkdocs.yml` 是 MkDocs 项目的配置文件，它用于定义和配置您的文档站点。在这个文件中，您可以设置站点名称、主题、导航结构、插件等。以下是 `mkdocs.yml`文件基本结构

```yml
site_name: Your Site Name
site_description: A description of your site
site_author: Your Name

nav:
  - Home: 'index.md'
  - info:
  	- Page 1: 'folder1/page1.md'
  	- Page 2: 'folder1/page2.md'

theme:
  name: 'material'
  # 更多主题设置（例如：颜色、字体等）

plugins:
  - search
  # 更多插件设置

```

## 用法

当需要补充wiki网站内容时，

1. 克隆master；
2. 在 `docs`路径下新建子文件夹，添加了说明文档；
3. 在 `mkdocs.yml`中的 `nav`添加相应名称与路径；
4. 使用gh-deploy。
