# HTML元素大集合

## a元素
### **描述**：
- a元素又称锚元素，可以通过**它的href属性**创建通向其他网页、文件、电子邮件地址、同一页面内的位置或任何其他URL的超链接。
- a中的内容应该指明链接的目标。如果存在**href**属性，当鼠标放到a元素上按下回车键就会相当于点击它。
  
### **例子**：
- ```
  <a href="https://example.com">Website</a>
  ```
- ```
  <a href="tel:+123456789">Phone</a>
  ```

### **属性**：
- download：导致浏览器将链接的URL视为下载资源。 
- href：超链接所指向的URL。
- target：指示在何处显示链接的URL。

  1. _self：当前页面。
  2. _blank：新窗口。
  3. _parent：父窗口，没有则与_self一致。
  4. _top：最顶级窗口，没有则与_self一致。




## abbr元素
### **描述**:
语义化元素，用于代表缩写，其可以与title属性提供完整的描述，当有title属性时有特殊的默认样式。

### **例子**：
- ```
  <p>大略过一遍<abbr title="文本标记语言">HTML</abbr>的所有元素</p>
  ```
- ```
  <p>大略过一遍<abbr>HTML</abbr>的所有元素</p>
  ```

### **属性**:
只有全局属性。


## address元素
### 描述：
语义化元素，表示其中内容提供了某个人或者组织等等的联系信息。

### 例子：
```
<address>
有事请联系我<a href="#">3249238@qq.com</a>
</address>
```

### 属性：
只有全局属性。


## article元素
### 描述：
语义化元素，表示文档、页面、应用或网站中的独立结构，其意在成为可复用的独立结构，如帖子、文章、评论等等。

### 例子：
```
<article>
    <h2>标题</h2>
    <section>内容</section>
</article>
```
### 属性：
只有全局属性。

## aside元素
### 描述：
语义化元素，表示一个和其余页面内容几乎无关的部分，可以单独拆分出来而不影响整体，通常表现为侧边栏。

### 例子：
```
<article>
  <h2>标题</h2>
  <section>内容</section>
  <aside>侧边栏</aside>
</article>
```
### 属性：
只有全局属性。


## audio元素
### 描述：
用于在文档中嵌入音频内容。可以使用**src属性**或者**source元素**来进行描述。
### 例子：
```
 <audio
    src="https://interactive-examples.mdn.mozilla.net/media/cc0-audio/t-rex-roar.mp3"
    controls autoplay>
  </audio>
```
### 属性：
- src：嵌入音频的URL。
- autoplay：布尔属性，尽快播放，不会等音频下载完。
- controls：提供可以控制音频播放的控制面板。
- currentTime：当前音频播放的位置。
- loop：无限循环播放。
- muted：静音播放。
- duration：音频的长度。

