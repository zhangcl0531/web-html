# web-html


>标题与段落

标题： h1,h2,h3....
段落：p

>列表

#### 无序列表
`<ul>` Unordered List
```html
<ul>
  <li></li>
  <li></li>
<ul>
```
ul和li一般嵌套使用

#### 有序列表
`<ol>` Ordered List

#### 嵌套列表

```html
<p>金州勇士队的全明星球员包括：<p>
<ul>
  <li>
    斯蒂芬·库里
    <ul>
      <li>微博：<a href="http://weibo.com/u/3432945104">@StephenCurry</a></li>
      <li>Twitter: <a href="https://twitter.com/stephencurry30">@StephenCurry30</a></li>
    </ul>
  </li>
  <li>凯文·杜兰特</li>
  <li>克莱·汤普森</li>
  <li>德雷蒙德·格林</li>
</ul>
```
>字体样式

#### 斜体
<em></em>

```html
<p>我<em>祝福</em>大家找到好工作。</p>
```

#### 加粗
<strong></strong>
```html
<p>靠你了，明天<strong>不要</strong>迟到!</p>
```

>描述列表

`<dl> <dt> <dd>`

```html
<dl>
  <dt>吃藕</dt>
  <dd>chi ou = 吃藕 = 丑 例句：被老板忽悠剪了个吃藕的发型。<dd>
  <dt>扩列<dt>
  <dd>扩充好友列表的简写，意为交朋友。<dd>
  <dt>狗带</dt>
  <dd>狗带 = go die, 表示去死。 例句：这节课太无聊了，我选择狗带。<dd>
</dl>
```

>超链接a标签

#### 简单链接
```html
<a href="https://github.com/zhangcl0531">张XX</a>
```

#### title 属性

```html
<a href="https://github.com/zhangcl0531" title="菜鸟自嗨网站">张XX</a>
```

#### 外部链接-链接跳转到新页面
将 target 设置成 _blank时，点击链接浏览器会新开一个 Tab 打开该网页

```html
<a href="https://github.com/zhangcl0531" title="菜鸟自嗨网站" target="_blank">张XX</a>
```
#### 返回顶部链接
```html
<a href="#">返回页面顶部</a>
```
#### 刷新网页
```html
<a href="">返回页面顶部</a>
```
#### 点击标签什么都不做
```html
<a href="javascript:;"></a>
```

#### 文档内部链接
用于定位到文档的某一部分,`<a>`的 href 要对应文档内某个元素的 id（id 的值在文档内要唯一）

```html
<a href="#email链接">Email链接</a>
```
#### 图片链接
```html
<a href="https://github.com/zhangcl0531" title="菜鸟自嗨网站">
   <img src="https://avatars3.githubusercontent.com/u/39626511?s=460&v=4" height="100">
</a>
```

#### 下载链接
```html
<a href="https://angular.io/resources/images/logos/angular/angular.svg" download>下载 Angular Logo</a>
```

#### 电话链接
```html
<a href="tel:+861588xxxxxxx">+86 1588xxxxxxx</a>
```

#### Email链接
```html
<a href="mailto:xidada@china.gov.cn">发封邮件给习大大</a> <br>
<a href="mailto:xidada@china.gov.cn?cc=pengliyuan@china.gov.cn">发封邮件给习大大并抄送第一夫人</a>
```

>图像img标签

#### 图片无法加载时显示文字
```html
<img src="https://vuejs.org/images/logo.png" alt="Vue.js logo" width="200">
```
#### 带说明的图像
```html
<figure>
  <img src="https://avatars3.githubusercontent.com/u/39626511?s=460&v=4"
       alt="张XX的GitHub头像"
       width="400"
       height="400">
  <figcaption>张XX的GitHub头像</figcaption>
</figure>
```

>表格table标签
```html
<table>
  <thead>
    <tr>
      <th>球员</th>
      <th>号码</th>
      <th>身高</th>
      <th>体重</th>
      <th>生日</th>
      <th>国籍</th>
      <th>出生地</th>
    <tr>
  </thead>
  <tbody>
    <tr>
      <td>勒布朗·詹姆斯</td>
      <td>23</td>
      <td>2.03米/6英尺8英寸</td>
      <td>113.4公斤</td>
      <td>1984年12月30日</td>
      <td colspan="2">美国</td>
    </tr>
    <tr>
      <td>凯里·欧文</td>
      <td>2</td>
      <td>1.91米/6英尺3英寸</td>
      <td>88公斤/193磅</td>
      <td>1992年3月23日</td>
      <td>美国/澳洲</td>
      <td>澳洲</td>
    </tr>
    <tr>
      <td>凯文·乐福</td>
      <td>0</td>
      <td>2.08米/6英尺10英寸</td>
      <td>110公斤/243磅</td>
      <td>1988年9月7日</td>
      <td colspan="2">美国</td>
    </tr>
  </tbody>
</table>
```
#### colgroup 设置表格宽度，样式
放在thead上面，表有多少行，就写多少col标签
```html
<colgroup>
   <col width=100>
   <col width=100 bgcolor=red>
   <col width=100>
   <col width=100>
</colgroup>
```
> 视频音频

#### 视频 <video>

```html
<video src="nba-finals2017-game-1.webm" controls>
  <p>你的浏览器不支持 HTML5 视频。</p> 
</video>
```
支持多种格式
- WebM - Chrome 和 Firefox
- MP4 - IE 和 Safari
- Ogg - 现在不怎么用了
```html
<video controls>
<source src="nba-finals2017-game-1.mp4" type="video/mp4">
<source src="nba-finals2017-game-1.webm" type="video/webm">
<p>你的浏览器不支持 HTML5 视频。</p> 
</video>
```
更多 video 特性
```html
<video controls width="400" height="400"
       autoplay loop muted
       poster="nab-finals.png">
    <source src="nba-finals2017-game-1.webm.mp4" type="video/mp4">
    <source src="nba-finals2017-game-1.webm" type="video/webm">
    <p>你的浏览器不支持 HTML5 视频。</p> 
</video>
```

#### 音频 <audio>
```html
<audio controls>
  <source src="viper.mp3" type="audio/mp3">
  <source src="viper.ogg" type="audio/ogg">
  <p>你的浏览器不支持 HTML5 音频。</p>
</audio>
```

>form表单
#### form标签属性
- action： 表单提交的地址
- method：提交保单的方法
- target：在何处打开action
- enctype:
  application/x-www-form-urlencoded
  text/plain：
  multipart/form-data

看代码吧，就知道了=。=
```html
<!DOCTYPE html>
<html>
<head>
  <title></title>
</head>
<body>
<div class="login">
  <input type="text" name="sex">
  <form action="/getInfo" method="get">
      <div class="submit">
      <button>提交😁</button> 会提交
    </div>
    <div class="username">
      <label for="username">姓名</label>
      <input id="username" type="text" name="username" value="ruo">
    </div>
    <div class="password">
      <label for="password">密码</label>
      <input id="password" type="password" name="password" placeholder="输入密码">
    </div>
    <div class="hobby">
      <label>爱好</label>
      <input type="checkbox" name="hobby" value="read" id="xxx"> <label for="xxx">读书</label> 点击字体也会选中
      <input type="checkbox" name="hobby" value="music"> 听歌
      <label><input type="checkbox" name="hobby" value="study"> 学习</label> 和上面效果相同
    </div>
    <div class="sex">
      <label>性别</label>
      <input type="radio" name="sex" value="男"> 男
      <input type="radio" name="sex" value="女"> 女
    </div>
    <div class="file">
      <input type="file" name="myfile" accept="image/png">
    </div>
    <div class="select">
      <select name="city">
        <option value="beijing">北京</option>
        <option value="shanghai" selected>上海</option>
        <option value="hangzhou">杭州</option>
      </select>
    </div>
    <div class="textarea">
      <textarea name="article">
         多行文本，注意和 type=text的区别
      </textarea>
      <input type="hidden" name="csrf" value="12345623fafdffdd">
        <input type="button" value="Buttom" /> 不会提交
        <input type="submit" value="Submit" /> 会提交
        <input type="reset" value="Reset" /> 重置输入
    </div>
  </form>
</div>
</body>
</html>
```

`<select name="city" multiple>  支持多选`<br>
`<textarea name="article"  resize:none> 设置不可改变文本框大小`

##### post vs get
- 表象不同，get把提交的数据url可以看到，post看不到
- 原理不同，get 是拼接 url， post 是放入http 请求体中
- 提交数据量不同，get最多提交1k数据，浏览器的限制。post理论上无限制，受服务器限制
- get提交的数据在浏览器历史记录中，安全性不好
- 场景不同，get 重在 "要", post 重在"给"

>hr 被水平线分隔的标题和段落
```html
<h1>This is header 1</h1>
<hr />
<p>This is some text</p>
```
![clipboard.png](https://upload-images.jianshu.io/upload_images/12361527-fe8bc42ec80d7da8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)