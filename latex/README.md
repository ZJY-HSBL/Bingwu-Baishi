# 《丙午稗史》· XeLaTeX 古典精装风格排印工程

本工程从《丙午稗史》现存 Markdown 底稿完整转制，含文言序、凡例、九卷（73则）、跋及题诗。封面采用原创深蓝烫金装饰画（为减少仓库体积，采用高质量 JPEG），书名由 XeLaTeX 字体独立排字。

## 编译

Linux 安装 TeX Live、xeCJK、ctex、Noto Serif CJK SC、TeXGyrePagella、DejaVu Sans、Noto Sans Javanese 等字体/宏包。在项目目录运行：

```bash
latexmk -xelatex -interaction=nonstopmode -halt-on-error main.tex
```

编译输出 `main.pdf`。亦可将整个 ZIP 上传 Overleaf，并设置 Compiler 为 XeLaTeX。项目中提供的 `丙午稗史_古典藏书版.pdf` 即已编译的成品。

## 文件

- `main.tex`：版式、封面、页眉页脚、目录、引用样式、主控文件。
- `chapters/`：序、凡例、九卷正文、跋以及扉页。
- `assets/cover-art.jpg`：原创封面插画。
- `source.md`：保留用于比对的 Markdown 底稿。

## 内容说明

本书是网络伪史言论的记录与批判研究，不代表编者赞同文中涉及的虚假信息、歧视、非人化或暴力言论。原文网名与来源尚未逐条独立验证。其内容无学术证据时不应作为历史或科学事实引用。

该版仅为个人数字编纂排印本，非经出版机构审定的正式出版物，不具有 ISBN。
