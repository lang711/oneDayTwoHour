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

## b元素
### 描述：
语义化元素，用于吸引读者注意到该元素内容上。

### 例子：
```
<section>震惊？女大学生无痛产子，竟是<b>神王</b></section>
```
### 属性：
只有全局属性。

## base元素
### 描述：
指定文档中所有包含相对URL的根URL，文档中只能有一个base元素。

### 例子：
```
//http://examp.com/abc
<base href="http://examp.com" target="_blank" />
<a href="/abc">随机地址</a> 
```
### 属性：
- href：用于文档中的基础URL，可以是绝对或相对路径。
- target：同a元素的target属性一致，也是所有链接的默认target。

## blockquote元素
### 描述：
代表其中文字是引用内容。

### 例子：
```
<blockquote cite="https://tools.ietf.org/html/rfc1149">
  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum omnis qui dignissimos laboriosam quasi totam aliquam amet quisquam,enim nisi atque, nihil porro eum ducimus itaque quaerat consequuntur
  </p>
</blockquote>
```
### 属性：
- cite：标注引用信息来源或相关信息的URL。


## button元素
### 描述：
表示一个可点击的按钮，可以用在**表单**或文档其他需要按钮的地方，但按钮的样式各个浏览器可能不同。

### 例子：
```
<section>
  <button autofocus disabled>按钮</button>
</section>
```
### 属性：
- type：
    - submit，将表单数据提交给服务器。
    - reset，重置表单元素。
    - button，表示普通按钮。
- disabled：禁用按钮。
- autofocus：获取焦点。



## canvas元素
### 描述：
被**javascript**用来绘制图形及图形动画。

### 例子：
```
 <canvas width="300" height="300"> 我是张三丰 </canvas>
```
### 属性：
- width：画布的宽度，默认300px。
- height：画布的高度，默认150px。

## del元素
### 描述：
表示文档中删除的文字内容。

### 例子：
```
 <p>删除的文字<del>我是张三丰</del></p>
```
### 属性：
只有全局属性。


## details元素
### 描述：
创建一个组件，切换成展开状态才会显示内含信息。
`<summary>`提供标签名。

### 例子：
```
<details>
  <summary>详情</summary>
  <span>我是张三丰啊</span>
</details>
```
### 属性：
- open：布尔属性，只有open才可见

## div元素
### 描述：
容器元素，在没有任何其他语义元素可用时使用。

### 例子：
```
<div>张三丰</div>
```
### 属性：
只有全局属性。


## dl元素
### 描述：
表示一个包含术语以及描述的列表，通常用于展示词汇。
`<dt>`元素表示术语，
`<dd>`元素表示描述。
### 例子：
```
 <dl>
  <dt>HTML</dt>
  <dd>标记语言</dd>
  <dt>JavaScript</dt>
  <dd>高级语言</dd>
</dl>
```
### 属性：
只有全局属性。


## em元素
### 描述：
语义化元素，表示强调，嵌套越深，强调程度越深。
### 例子：
```
 <p>我是<em>张三丰</em></p>
```
### 属性：
只有全局属性。


## embed元素
### 描述：
将外部内容嵌入文档中的指定位置。此内容由外部程序或插件提供。
### 例子：
```
  <embed src="https://picsum.photos/200/300" type="" />
  <embed src="https://chat.baidu.com/" />
```
### 属性：
- type：mime类型。
- src：嵌套资源的URL。
- width：显示的宽度。
- height：显示的高度。


## fieldset元素
### 描述：
用于对表单中的控制元素进行分组，当然也可以在表单外使用。
`<legend>`元素表示分组标题。
### 例子：
```
<fieldset>
    <legend>张三</legend>
    <div>年龄：20</div>
    <div>性别：男</div>
</fieldset>
```
### 属性：
- disabled：子代表单元素会继承这个属性。
- form：与`<form>`表单关联。
