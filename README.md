# 介绍
你好！我是Autumn。本网页基于Jekyll主题Chirpy模板搭建，感谢原作者提供的模板。下方是原文件中关于Chirpy Starter的介绍。

- 本人网页地址： [AuTuMnnn网页](https://autumnnn458.github.io/)
- Chirpy主题地址: [Chirpy](http://jekyllthemes.org/themes/jekyll-theme-chirpy/)
- Chirpy demo: [Chirpy demo](https://chirpy.cotes.page/)

再次感谢chirpy作者提供的网页模板，以及github pages提供的在线网页部署服务。


# 使用注意事项
如果你想使用Chirpy Starter搭建自己的网页，你可能需要注意以下内容，这些内容都是我在开发时遇到的一些问题：
1. _posts文件夹中的文件只能以`YYYY-MM-DD-title`形式命名，文件名内的空格以`-`连接，少了时间或多了空格都会使得pages部署失败。
2. _posts文件夹中的markdown文档基本遵循markdown语法，但也有需要注意的地方：
- 关于catagories: 要在文章前的注释中清楚写好，在网页的catagories部分会按照文件夹分类。
- 关于代码：使用的代码块中标识的语言要用全小写。例如：下面这两个代码块在github上都能正常显示，但是在网页中只有第二种即` ```python ``` `可以正常显示。
第一块：
```Python
import ...
```
第二块：
```python
import ...
```


# Chirpy Starter

[![Gem Version](https://img.shields.io/gem/v/jekyll-theme-chirpy)][gem]&nbsp;
[![GitHub license](https://img.shields.io/github/license/cotes2020/chirpy-starter.svg?color=blue)][mit]

When installing the [**Chirpy**][chirpy] theme through [RubyGems.org][gem], Jekyll can only read files in the folders
`_data`, `_layouts`, `_includes`, `_sass` and `assets`, as well as a small part of options of the `_config.yml` file
from the theme's gem. If you have ever installed this theme gem, you can use the command
`bundle info --path jekyll-theme-chirpy` to locate these files.

The Jekyll team claims that this is to leave the ball in the user’s court, but this also results in users not being
able to enjoy the out-of-the-box experience when using feature-rich themes.

To fully use all the features of **Chirpy**, you need to copy the other critical files from the theme's gem to your
Jekyll site. The following is a list of targets:

```shell
.
├── _config.yml
├── _plugins
├── _tabs
└── index.html
```

To save you time, and also in case you lose some files while copying, we extract those files/configurations of the
latest version of the **Chirpy** theme and the [CD][CD] workflow to here, so that you can start writing in minutes.

## Usage

Check out the [theme's docs](https://github.com/cotes2020/jekyll-theme-chirpy/wiki).

## Contributing

This repository is automatically updated with new releases from the theme repository. If you encounter any issues or want to contribute to its improvement, please visit the [theme repository][chirpy] to provide feedback.

## License

This work is published under [MIT][mit] License.

[gem]: https://rubygems.org/gems/jekyll-theme-chirpy
[chirpy]: https://github.com/cotes2020/jekyll-theme-chirpy/
[CD]: https://en.wikipedia.org/wiki/Continuous_deployment
[mit]: https://github.com/cotes2020/chirpy-starter/blob/master/LICENSE
