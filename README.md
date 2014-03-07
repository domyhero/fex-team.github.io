
## 这什么？

这是 FEX 团队对外 Blog 的源码，团队成员将文档提交到这里就能在 <http://fex.baidu.com> 上显示。

## 如何写？

### 环境搭建

这个 Blog 系统是基于 [jekyll](http://jekyllrb.com/) 搭建的，为了方便本地编辑和看效果，首先需要在本机安装 jekyll 环境，其中的 gem 命令是 [Ruby](https://www.ruby-lang.org/)  语言的包管理工具。

    gem install jekyll

接着通过如下命令就能在本地查看效果了:

    jekyll serve --watch

### 新建草稿

新文章编写时请先浏览 `_drafts` 目录，这里存放着还未完成的草稿，它不会在首页显示，请参考里面的 `2014-05-06-empty.md` 文件，新建文件名要遵循这样的格式，以日期开头，后面接着是文章的对外 url 子路径，中间以 `-` 分隔，后续标题有多个单词时也以 `-` 作为分隔符。

### 个人信息

每篇文章都会附上个人信息，所以请先编辑 `_data\authors.yml` 文件，按照其中的格式新增一个，需要注意以下 2 点：

* 这是 YAML 格式，每行的开头是两个空格，而不是 TAB。
* `author` 字段需要和你所写文章开头的 `author` 属性保持一致，这样才能正确展现。

### 图片存放地

请将图片放在 `img` 目录里，每篇文章新建一个目录，在文章中的引用方式为：

    ![](/img/<文章名>/xx.png)

### 发布

如果觉得文章可以对外展示了，就将它移到 `_posts` 目录下，提交 github 后就马上生效了。

### 小技巧

* jekyll 最终生成的文件会放在 `_site` 目录下，可以通过浏览这个目录来确认效果。
* img 目录的主要用途是放图片，但也可以放其它文件静态，如 zip 等

## 写什么？

虽然外界会认为这是团队 Blog，但实际上它是每个团队成员的个人分享，每篇文章都只代表你自己的观点，所以如果你觉得有什么是值得分享的，请不要犹豫，马上就写吧，借助这个平台来提升自己的影响力。

具体内容形式将包括但不限于：

* 技术介绍、经验总结
* FEX 新开源项目及升级版本介绍
* 优秀文章的翻译
* 优秀资源（书籍、开源项目）等的推荐
* 内部分享的 PPT（推荐使用 [Speaker Deck](https://speakerdeck.com/) 存放）

另外，如果你对目前界面的哪些细节不满意，也欢迎直接修改相关源码。

### 对于写作风格的约定

请参考[FEX 写作风格](https://github.com/fex-team/styleguide/blob/master/writing.md)


