# 贵州大学选修课课程报告LaTeX模板（非官方）

标签（空格分隔）： LaTeX GZU

---
[TOC]
##说明
　　本模板为作者学习LaTeX后的自制作品，主要由`report.tex`单文件组成，不涉及学校专用宏包。想要查看生成效果请打开`report.pdf`文件进行查看。具体说明如下：
###环境
|项目|内容|
|:-:|:-:|
|语言|LaTeX|
|编译环境|XeLaTeX|
|版本|1.0|
###主要宏包
|名称|说明|
|:-:|:-:|
|\documentclass{ctexart}|CTeX套件的文档包，用以中文排版|
|\usepackage{ulem}   |%用于字体加强
|\usepackage{amsmath}    |%用于数学公式
|\usepackage{graphicx}   |%用于插入图像
|\usepackage{subfig} |%用于排列图像
|\usepackage{booktabs}   |%用于制作三线表格
|\usepackage{multirow}   |%用于表格跨行
|\usepackage{fancyhdr}   |%用于设置页面格式
|\usepackage{verbatim}   |%用于打印代码（原文输出）
|\usepackage{setspace}   |%设置行距
其中，设置页面为A4纸张，默认字号为12pt。
##页面设置
主要分成了四大页面，包括封面、目录、正文、参考文献。
* 封面
    * 封面部分导入`pic`文件夹下的两张标志图片。个人信息则由表格生成，由于掌控不好间距，所以代码中出现了很多`\newline`以及`\\`换行符。（我也很绝望啊---来自新手的咆哮\_(:з」∠)\_）。
    * 其中由于封面底部需要署名日期，故加上了`\Date`命令此命令有三个参数，具体用法及声明见下方代码，由年月日三个参数组成。
```latex
\newcommand{\Date}[3]{\heiti\zihao{2} #1年#2月#3日}%生成日期
\Date{2017}{2}{19}
```
* 目录
普通格式,生成时记得点两下XeLaTeX编译键。
* 正文
运用了小技巧简化首行缩进：`Shift + Space`切换全角符号后点两下Space键即可。
* 参考文献
普通格式。
##声明
　　请大家忽视报告内容，请大家忽视报告内容，请大家忽视报告内容。。。写的不咋地，主要是阐述报告的样式。
　　由于作者是初学（两天速成），所以做出的东西甚是简陋，希望有经验的同学们可以参与进来一同完善。也可以提交issue，报告缺陷或申请pull request，修正文档内容或添加一些实用的LaTeX模板，比如数模、毕业论文等等。期待大家的参与。
##联系作者
Spico（spico@qq.com）