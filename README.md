# Die Bond Docs

## 介绍

Die Bond 项目文档

## MkDocs 使用教程

### 1、Installation

```bash
pip install mkdocs-material
```

### 2、Creating

```bash
mkdocs new .
```

### 3、Configuration

```bash
- `site_name`：网站的名称是 "MkDocs YouTube Tutorial"。
- `site_url`：网站的 URL 是 https://james-willett.github.io/mkdocs-material-youtube-tutorial/。
- `theme`：网站使用的主题是 Material 主题，配置了一些功能和配色方案。
  - `name`：主题名称为 Material。
  - `features`：包含了一系列功能，如导航、搜索等。
  - `language`：语言设置为英语。
  - `palette`：配色方案设置，包括两种方案，分别为默认的 teal 和 slate。
- `plugins`：启用了一个社交插件，用于显示社交媒体链接。
- `extra`：额外的配置信息，包括社交媒体的图标和链接。
- `markdown_extensions`：Markdown 扩展，用于增强 Markdown 文档的功能，如代码高亮、注释、数学公式等。
- `copyright`：版权信息，包括版权年份和作者信息。
```

```bash
site_name: Markdown book
site_description: Describe what your site is about  # 设置文档网站的描述
site_url: 'https://example.com'  # 设置文档网站的 URL

theme:
  name: material

  language: zh  # zh en
  palette:
    - scheme: default
      toggle:
        icon: material/toggle-switch-off-outline 
        name: Switch to dark mode
      primary: teal
      accent: purple 
    - scheme: slate 
      toggle:
        icon: material/toggle-switch
        name: Switch to light mode    
      primary: teal

markdown_extensions:
  - pymdownx.highlight:
      anchor_linenums: true
  - pymdownx.inlinehilite
  - pymdownx.snippets
  - admonition
  - pymdownx.arithmatex:
      generic: true
  - footnotes
  - pymdownx.details
  - pymdownx.superfences
  - pymdownx.mark
  - attr_list
  - pymdownx.emoji:
      emoji_index: !!python/name:materialx.emoji.twemoji
      emoji_generator: !!python/name:materialx.emoji.to_svg
```

### 4、Previewing as you write

```bash
mkdocs serve
```

### 5、编译HTML

```bash
mkdocs build
```