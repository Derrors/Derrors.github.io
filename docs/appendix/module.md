下述均为个人理解，不保证准确性

## **python markdown**

---

是用python写的markdown模块，用这模块可以将markdown文本渲染成html，比如：

```text
>>> import markdown
>>> text = '''
... # abc
... ```go
... import "fmt"
... ```
...
... ## sss
...
... - xxx
... - yyy
... '''
>>> html = markdown.markdown(text)
>>> print html
<h1>abc</h1>
<p><code>go
import "fmt"</code></p>
<h2>sss</h2>
<ul>
<li>xxx</li>
<li>yyy</li>
</ul>
```

同时markdown模块内置一些扩展，有：

- abbr.py
- admonition.py
- attr_list.py
- codehilite.py
- def_list.py
- extra.py
- fenced_code.py
- footnotes.py
- headerid.py
- meta.py
- nl2br.py
- sane_lists.py
- smart_strong.py
- smarty.py
- tables.py
- toc.py
- wikilinks.py

## **pymdownx**

---

是python的一个模块，扩展了markdown的功能，比如emoji图标、可折叠的文本框等，pymdownx也是调用markdown模块做事，pymdownx包含以下功能：

- arithmatex.py
- b64.py
- betterem.py
- caret.py
- critic.py
- details.py
- emoji.py
- emoji1_db.py
- escapeall.py
- extra.py
- extrarawhtml.py
- gemoji_db.py
- github.py
- highlight.py
- inlinehilite.py
- keymap_db.py
- keys.py
- magiclink.py
- mark.py
- pathconverter.py
- plainhtml.py
- progressbar.py
- slugs.py
- smartsymbols.py
- snippets.py
- superfences.py
- tasklist.py
- tilde.py
- twemoji_db.py
- util.py

## **mkdocs**

---

是用python编写的，包括mkdocs主题及命令行工具，mkdocs调用python markdown来渲染html，其中重写了少部分基础功能，比如toc，以达到符合mkdocs主题效果；mkdocs也内置一种主题，就叫mkdocs，同时也内置支持readthedocs，并且mkdocs也支持自定义主题。mkdocs主要就是一个集成器，通过这个工具来简化渲染、部署、使用、模块调用、主题调用

## **material**

---

是python的一个模块，是符合mkdocs规范的自定义主题，可以通过pip install mkdocs-material来下载，这个模块里面都是一些js、css、html文件

material这个模块名和主题风格，是来自于google material，即google定义的一种通用风格，用于兼容不同分辨率下的页面展示，即只要符合这种谷歌风格的，一处编写，处处使用（在pc、手机上都可以用，即会根据分辨率自动调整页面展示）

material主题对python markdown的一些内置扩展和pymdownx的功能做了主题效果优化，以便更优美，内置的有：

- 支持的python markdown扩展有：Admonition、CodeHilite、Footnotes、Metadata、Permalinks

- pymdownx有：Arithmatex、BetterEM、Caret、Critic、Details、Emoji、InlineHilite、MagicLink、Mark、SmartSymbols、SuperFences、Tasklist、Tilde
