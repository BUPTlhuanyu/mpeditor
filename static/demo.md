# 欢迎使用 MPEditor Markdown 编辑阅读器

**MPEditor**是专注于微信公众号的编辑阅读器，利用MPEditor可以使用 **Markdown** 语法编写微信公众号文章，编辑完后可以复制到公众号发布平台直接发布，真正的实现即看即所得：

* 更加贴合微信UI标准
* 支持live preview 
* 支持同步滚动
* 支持语法高亮
* 支持emoji表情

> MPEditor解决了微信公众号编辑中遇见的一些编辑问题，增加了「工（ma）程（nong）师（men）」经常遇见的代码高亮、emoji和粗糙的审美问题。希望你会喜欢这个编辑器！


## 什么是 Markdown

Markdown 是一种方便记忆、书写的纯文本标记语言，用户可以使用这些标记符号以最小的输入代价生成极富表现力的文档：譬如您正在阅读的这份文档。它使用简单的符号标记不同的标题，分割不同的段落，**粗体** 、 *斜体* 、~~delete~~ 某些文字。@@@@MPEditor@@@@ 使用了 `showdown` 语法[^2]

# 标题样式：标题一，太个性了，一般别用了！
## 标题二
### 标题三
#### 标题四
##### 标题五，不常用
###### 标题六，不常用


# 1. 基本列表样式

* 偶是个无序列表
    - 我是个二级无序列表
* 真巧啊我也是个无序列表


1. 我是个有序列表啊
2. 嗯，me too~
3. markdown so easy! 妈妈再也不用担心我的**学习**了

# 2. 制作一份待办事宜

- [ ] 自动保存
- [ ] 增加顶部工具栏：复制、github
- [ ] 增加QQ音乐markdown语法支持
- [x] 增加emoji语法支持
- [ ] 增加底部公众号关注语法
- [x] wechat标准UI样式修改
- [x] 修改markdown demo

# 3. 高亮一段代码

```js
// 新语法检测
import $ from 'jQuery'
$(document).on('click', ()=>{
  let that = this
  console.log(that)
})

var aceEditor = new ace.editor('#id')

$(function(){
  $('div').html('I am a div.');
});
```

上面是 `JavaScript`，下面是 `php`：

```php
echo 'hello,world'
```

# 4. 绘制表格
下面是个普通的表格
| 公众号 | id | 备注 |
|-----|-----|------|
| 三水清 | sanshuiqing123   | 作者很帅 |
| 博客 | http://js8.in   | 程序媛鼓励师 |


支持另外一种语法：
公众号        | id/网址       | 备注
------------ | ----------   | ------
三水清 | sanshuiqing123 | 作者很帅 
博客 | http://js8.in   | 程序媛鼓励师 


下面的表格支持左右对齐：
| h1    |    h2   |      h3 |
|:------|:-------:|--------:|
| 100   | a[^1]  | b[^2] |
| *foo* | **bar** | ~~baz~~ |

# 5. 链接和图片

* MPEditor：https://github.com/ksky521/mpeditor[^1]
* wiki：[点击查看wiki](https://github.com/ksky521/mpeditor/wiki)

下面是个「三水清」的微信公众号二维码，欢迎扫描关注：
![关注三水清](https://raw.githubusercontent.com/ksky521/mpeditor/master/static/qrcode_for_me.jpg)

换个小点的头像
![关注三水清](https://raw.githubusercontent.com/ksky521/mpeditor/master/static/qrcode_for_me.jpg =120x120)

# 6. 还支持emoji！

* Unicode支持：😈 💗 😄 🐂 👍
* github版本支持：:octocat: :cn: :red_car: :muscle: :smile: :sunglasses:

# 7. 自定义样式

* @@绿色 green@@ **@@绿色 green@@**
* @@@红色 warn@@@
* @@@@蓝色 blue@@@@
* @@@@@黄色 yellow@@@@@

再一次感谢您花费时间阅读这份欢迎稿！

作者[@三水清][^3]
2017年02月19日

### Footnotes

[^1]: https://github.com/ksky521/mpeditor
[^2]: https://github.com/showdownjs/showdown/wiki/Showdown's-Markdown-synta
[^3]: http://weibo.com/sanshuiqing
