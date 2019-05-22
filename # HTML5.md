# HTML5
## 一个HTML5的例子
```
<!DOCTYPE HTML>
<html>
<body>

<video width="320" height="240" controls="controls">
  <source src="movie.ogg" type="video/ogg">
  <source src="movie.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

</body>
</html>
```
## HTML 5简介
### 什么是 HTML5？
HTML5 将成为 HTML、XHTML 以及 HTML DOM 的新标准。
HTML 的上一个版本诞生于 1999 年。自从那以后，Web 世界已经经历了巨变。
HTML5 仍处于完善之中。然而，大部分现代浏览器已经具备了某些 HTML5 支持。
### HTML5是如何起步的？
HTML5 是 W3C 与 WHATWG 合作的结果。

WHATWG 致力于 web 表单和应用程序，而 W3C 专注于 XHTML 2.0。在 2006 年，双方决定进行合作，来创建一个新版本的 HTML。

为 HTML5 建立的一些规则：

+ 新特性应该基于 HTML、CSS、DOM 以及 JavaScript。
+ 减少对外部插件的需求（比如 Flash）
+ 更优秀的错误处理
+ 更多取代脚本的标记
+ HTML5 应该独立于设备
+ 开发进程应对公众透明

### 新特性
HTML5 中的一些有趣的新特性：
+ 用于绘画的 canvas 元素
+ 用于媒介回放的 video 和 audio 元素
+ 对本地离线存储的更好的支持
+ 新的特殊内容元素，比如 article、footer、header、nav、section
+ 新的表单控件，比如 calendar、date、time、email、url、search

## HTML5新增标签

| **标签**     | **描述**                                           |
| ------------ | -------------------------------------------------- |
| <article>    | 定义article                                        |
| <aside>      | 定义页面内容之外的内容。                           |
| <audio>      | 定义声音内容。                                     |
| <bdi>        | 定义文本的文本方向，使其脱离其周围文本的方向设置。 |
| <canvas>     | 定义图形。                                         |
| <command>    | 定义命令按钮。                                     |
| <datalist>   | 定义下拉列表。                                     |
| <details>    | 定义元素的细节。                                   |
| <embed>      | 定义外部交互内容或插件。                           |
| <figcaption> | 定义   figure 元素的标题。                         |
| <figure>     | 定义媒介内容的分组，以及它们的标题。               |
| <footer>     | 定义   section 或 page 的页脚。                    |
| <header>     | 定义   section 或 page 的页眉。                    |
| <hgroup>     | 定义有关文档中的   section 的信息。                |
| <keygen>     | 定义生成密钥。                                     |
| <main>      | 定义文档的主要内容。                         |
| <mark>       | 定义有记号的文本。                                 |
| <meter>      | 定义预定义范围内的度量。                           |
| <nav>        | 定义导航链接。                                     |
| <output>     | 定义输出的一些类型。                               |
| <progress>   | 定义任何类型的任务的进度。                         |
| <rp>         | 定义若浏览器不支持 ruby 元素显示的内容。           |
| <rt>         | 定义 ruby 注释的解释。                             |
| <ruby>       | 定义 ruby 注释。                                   |
| <section>    | 定义   section。                                   |
| <source>     | 定义媒介源。                                       |
| <summary>    | 定义   details 元素的标题。                        |
| <time>       | 定义日期/时间。                                    |
| <track>      | 定义用在媒体播放器中的文本轨道。                   |
| <video>      | 定义视频。                                         |

### article

**1、定义和用法：**

<article> article元素代表文档、页面或应用程序中独立的、完整的、可以独自被外部引用的内容。

可能的 article 实例：

- 论坛帖子
- 报纸文章
- 博客条目
- 用户评论

**2、实例**
```
<article>
      <header>
            <h1>article元素使用方法</h1>
            <p>发表日期：<time pubdate="pubdate">2019/05/20</time></p>
      </header>
      <p>article元素是什么？怎样使用article元素？……</p>
      <section>
            <h2>评论</h2>
            <article>
                  <header>
                        <h3>发表者：Felixlu</h3>
                        <p><time pubdate datetime="2019-05-20T:21-26:00">1小时前</time></p>
                  </header>
                  <p>这篇文章很不错啊，顶一下！</p>
            </article>
            <article>
                  <header>
                        <h3>发表者：神秘唯一</h3>
                        <p><time pubdate datetime="2019-05-20T:21-26:00">1小时前</time></p>
                  </header>
                  <p>这篇文章很不错啊，对article解释的很详细</p>
            </article>
      </section>
</article>
```
### section

**1、定义和用法：**

section元素用于对网站或应用程序中页面上的内容进行分块。一个section元素通常由内容及其标题组成。但section元素并非一个普通的容器元素；当一个内容需要被直接定义样式或通过脚本定义行为时，推荐使用div而非section元素。section元素中的内容可以单独存储到数据库中或输出到word文档中。

**2、实例**

通常不推荐为那些没有标题的内容使用section元素。
section元素的作用是对页面上的内容进行分块，或者说对文章进行分段，请不要与有着自己的完整的、独立的内容的article元素混淆。
```
<section>
      <h1>section元素使用方法</h1>
      <p>什么时候用section元素？怎样合理使用section元素?</p>
</section>

<article>
      <h1>article元素与section元素的使用方法</h1>
      <p>何时使用article元素？何时使用section元素…..</p>
      <section>
            <h2>article元素使用方法</h2>
            <p>article元素代表文档、页面或应用程序中独立的、完整的、可以独自被外部引用的内容。</p>
      </section>
      <section>
            <h2>section元素使用方法</h2>
            <p> section元素用于对网站或应用程序中页面上的内容进行分块。</p>
      </section>
</article>
```
**3、section 使用禁忌**

+ 不要将section元素用作设置样式的页面容器，那是div元素的工作。
+ 如果article元素、aside元素或nav元素更符合使用条件，不要使用section元素。
+ 不要为没有标题的内容区块使用section元素。

**4、section 与 article 的区别**

在HTML5中，article元素可以看成是一种特殊类型的section元素，它比 section元素更强调独立性。即section元素强调分段或分块，而article强调独立性。具体来说，如果一块内容相对来说比较独立的、完整的时候，应该使用article元素，但是如果你想将一块内容分成几段的时候，应该使用section元素。另外，在HTML5中，div元素变成了一种容器，当使用CSS样式的时候，可以对这个容器进行一个总体的CSS样式的套用。

### aside

**1、定义和用法**

HTML<aside>元素表示一个页面的一部分， 它的内容跟这个页面的其它内容的关联性不强，或者是没有关联，单独存在。<aside>元素通常显示成侧边栏(sidebar)或一些插入补充内容。通常用来在侧边栏显示一些定义，比如目录、索引、术语表等；也可以用来显示相关的广告宣传，作者的介绍，Web应用，相关链接，当前页内容简介等。

不要使用<aside>元素标记括号中的文字，因为这种类型的文本被认为是主内容的一部分。

**2、实例**
```
<article>  
  <p>  
    The Disney movie <em>The Little Mermaid</em> was   
    first released to theatres in 1989.   
  </p>  
  <aside>  
    The movie earned $87 million during its initial release.   
  </aside>  
  <p>  
    More info about the movie...   
  </p>  
</article>
```
### main

**1、定义和用法**

<main> 标签规定文档的主要内容。

<main> 元素中的内容对于文档来说应当是唯一的。它不应包含在文档中重复出现的内容，比如侧栏、导航栏、版权信息、站点标志或搜索表单。

**注释：**在一个文档中，不能出现一个以上的 <main> 元素。<main> 元素不能是以下元素的后代：<article>、<aside>、<footer>、<header> 或 <nav>。

**2、实例**

```
<main>
  <h1>Web Browsers</h1>
  <p>Google Chrome、Firefox 以及 Internet Explorer 是目前最流行的浏览器。</p>

  <article>
    <h1>Google Chrome</h1>
    <p>Google Chrome 是由 Google 开发的一款免费的开源 web 浏览器，于 2008 年发布。</p>
  </article>

  <article>
    <h1>Internet Explorer</h1>
    <p>Internet Explorer 由微软开发的一款免费的 web 浏览器，发布于 1995 年。</p>
  </article>

  <article>
    <h1>Mozilla Firefox</h1>
    <p>Firefox 是一款来自 Mozilla 的免费开源 web 浏览器，发布于 2004 年。</p>
  </article>
</main> 
```

### header

**1、定义和用法**

标签 <header> 定义文档的页眉（介绍信息）。

**2、实例**
```
<header>
  <h1>Welcome to my homepage</h1>
  <p>My name is Donald Duck</p>
</header>
<p>The rest of my home page...</p>
```
### footer

**1、定义和用法**

标签 <footer> 定义文档或节的页脚。

元素 <footer> 应当含有其包含元素的信息。

页脚通常包含文档的作者、版权信息、使用条款链接、联系信息等等。

您可以在一个文档中使用多个 <footer> 元素。

**2、实例**

```
<footer>
  <p>Posted by: GP-1011</p>
  <p>Contact information: <a href="mailto:someone@example.com">someone@example.com</a>.</p>
</footer>
```

### nav

**1、定义和用法**

`<nav>`是与导航相关的，所以一般用于网站导航布局。同时完全就像使用`div`标签、`span`标签一样来使用`<nav>`标签，可添加`id`或`class`。而与`div`标签又有不同处是，此标签一般只用于导航相关地方使用，所以在一个html网页布局中可能就使用在导航条处，或与导航条相关的地方布局使用。

**2、实例**
```
<nav> 
  <ul> 
    <li>首页</li> 
    <li>栏目名称</li> 
    <li>联系我们</li> 
  </ul> 
</nav> 
```

### datalist

**1、定义和用法**

<datalist> 标签定义选项列表。与 input 元素配合使用该元素，来定义 input 可能的值。

datalist 及其选项不会被显示出来，它仅仅是合法的输入值列表。

使用 input 元素的 list 属性来绑定 datalist。

**2、实例**
```
<input id="myCar" list="cars" />

<datalist id="cars">
  <option value="BMW">
  <option value="Ford">
  <option value="Volvo">
</datalist>
```

### command

**1、定义和用法**

在HTML5中，<command>标签是用来表示用户能够调用的命令，可以定义命令按钮，比如单选按钮、复选框或按钮。<command>标签在<menu>元标签中才是可见的，它还可以规定键盘快捷键。<command> 标签是html 5中新增标签，目前只有在IE 9中支持。

**2、实例**
```
<menu>
  <command type="command" label="Save" onclick="save()">Save</command>
</menu>
```

### details & summary

**1、定义和用法**

`<details>` 标签 用于描述文档或文档某个部分的细节，与 <summary> 标签 配合使用可以为 details 定义标题。标题是可见的，用户点击标题时，会显示出 details。
`<details>` 标签 拥有 open 属性，"details" 元素默认是隐藏的，设置 open 属性后，可以定义"details" 元素默认可见，与checkbox定义checked属性是一个道理。

**2、实例**
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Title</title>
    <style>
        ::-webkit-details-marker{
            display:none;
        }
        ::-moz-list-bullet {
            font-size: 0;
            float: left;
        }
        summary{
            font-weight:bolder;
            cursor:pointer;
            user-select: none;
            outline: 0;
        }
        li{
            list-style: none;
        }
    </style>
</head>
<body>
    <details>
        <summary>商品管理</summary>
        <li>商品列表</li>
        <li>添加商品</li>
    </details>
    <details>
        <summary>品牌管理</summary>
        <li>品牌列表</li>
        <li>添加品牌</li>
    </details>
    <details>
        <summary>分类管理</summary>
        <li>分类列表</li>
        <li>添加分类</li>
    </details>
</body>
</html>
```
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>details & summary</title>
  <style>
    div {
        width: 7%;
        margin: 0 auto;
        text-align: center;
    }
    ::-webkit-details-marker {
        display:none;
    }
    ::-moz-list-bullet {
        font-size: 0;
        float: left;
    }
    details {
        position:relative;
        background:#f5f5f5;
    }
    summary {
        font-weight:bolder;
        cursor:pointer;
        user-select: none;
        outline: 0;
    }
    li {
        border:1px solid #eee;
        border-top : 0;
        list-style: none;
    }
    /* 实现动画的原理 */
    summary::after {
        content: '';
        width: 0;
        height: 0;
        line-height: 0;
        font-size: 0;
        border-left: 5px dashed transparent;
        border-right: 5px dashed transparent;
        border-top: 5px solid #000;
        position: absolute;
        top: 44%;
        right: 8%;
        transition:.3s ease-out;
    }
    [open] summary::after {
        transform:rotate(180deg)
    }
    ul {
        max-height: 0;
        padding:0;
        margin-top:0;
        transition: .3s ease-out;
        overflow: hidden;
    }
    [open] + ul {
        max-height: 60px;
    }
  </style>
</head>
<body>
    <div>
        <details open>
            <summary>商品管理</summary>
        </details>
        <ul>
            <li>商品列表</li>
            <li>添加商品</li>
        </ul>
    </div>
    <div>
        <details open>
            <summary>品牌管理</summary>
        </details>
        <ul>
            <li>品牌列表</li>
            <li>添加品牌</li>
        </ul>
    </div>
    <div>
        <details open>
            <summary>分类管理</summary>
        </details>
        <ul>
            <li>分类列表</li>
            <li>添加分类</li>
        </ul>
    </div>
</body>
</html>
```

### hgroup

**1、定义和用法**

hgroup元素是将标题和他的子标题进行分组的元素。hgroup元素一般会把h1-h6的元素进行分组，比如在一个内容区块的标题和他的子标题算是一组。通常情况下，文章只有一个主标题时，是不需要hgroup元素的。

**2、实例**
```
<article>
  <header>
    <hgroup>
      <h1>文章主标题</h1>
      <h2>文章子标题</h2>
    </hgroup>
    <p><time datetime=”2019-05-20”>2019年05月20日</time></p>
  </header>
  <p>文章正文</p>
</article>
```

### figure & figcaption

**1、定义和用法**

`<figure>`  标签规定独立的流内容（图像、图表、照片、代码等等）。

figure 元素的内容应该与主内容相关，但如果被删除，则不应对文档流产生影响。

**2、实例**

hover 例子：https://tympanus.net/Development/HoverEffectIdeas/index2.html
```
<div class="hover-area area-Julia">
  <img src="imgs/21.jpg" height="360" width="480">
  <h3>PASSIONATE<strong>JULIA</strong></h3>
  <ul>
    <li>Julia dances in the deep dark.</li>
    <li>She loves the smell of the ocean</li>
    <li>And dives into the morning light</li>
  </ul>
</div>
```
VS
```
<figure class="effect-julia">
  <img src="img/21.jpg" alt="img21"/>
  <figcaption>
    <h2>Passionate <span>Julia</span></h2>
    <div>
      <p>Julia dances in the deep dark</p>
      <p>She loves the smell of the ocean</p>
      <p>And dives into the morning light</p>
    </div>
    <a href="#">View more</a>
  </figcaption>			
</figure>
```

### mark

**1、定义和用法**

<mark> 标签定义带有记号的文本。请在需要突出显示文本时使用 <m> 标签。

**2、实例**
```
<p>Do not forget to buy <mark>milk</mark> today.</p>
```

### time

**1、定义和用法**

<time> 标签定义公历的时间（24 小时制）或日期，时间和时区偏移是可选的。

该元素能够以机器可读的方式对日期和时间进行编码，这样，举例说，用户代理能够把生日提醒或排定的事件添加到用户日程表中，搜索引擎也能够生成更智能的搜索结果。

**2、实例**
```
<p>我们在每天早上 <time>9:00</time> 开始营业。</p>
<p>我在 <time datetime="2019-02-14">情人节</time> 有个约会。</p>
```

### output

**1、定义和用法**

<output> 标签定义不同类型的输出，比如脚本的输出。

**2、实例**

```
<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">0
   <input type="range" id="a" value="50">100
   +<input type="number" id="b" value="50">
   =<output name="x" for="a b"></output>
</form> 
```

### progress

**1、定义和用法**

<progress> 标签标示任务的进度（进程）。

**2、实例**

```
<progress value="22" max="100"></progress>

样式：
progress {
   color:orange; /*兼容IE10的已完成进度背景*/
   border:none;
   background: #d7d7d7;/*这个属性也可当作Chrome的已完成进度背景，只不过被下面的::progress-bar覆盖了*/      
}

progress::-webkit-progress-bar {
   background: #d7d7d7;
}

progress::-webkit-progress-value,
progress::-moz-progress-bar
{
  background: orange;
}
```

### meter

**1、定义和用法**

<meter> 标签定义已知范围或分数值内的标量测量。也被称为 gauge（尺度）。

例子：磁盘用量、查询结果的相关性，等等。

**注释：**<meter> 标签不应用于指示进度（在进度条中）。如果标记进度条，请使用 <progress> 标签。

**2、实例**
```
<meter value="3" min="0" max="10">十分之三</meter>
<meter value="0.6">60%</meter> 
```

### keygen

**1、定义和用法**

<keygen> 标签规定用于表单的密钥对生成器字段。

当提交表单时，私钥存储在本地，公钥发送到服务器。

**2、实例**
```
<form action="demo_keygen.do" method="get">
  Username: <input type="text" name="usr_name" />
  Encryption: <keygen name="security" />
  <input type="submit" />
</form>
```

### embed

**1、定义和用法**

embed可以用来插入各种多媒体，格式可以是 Midi、Wav、AIFF、AU、MP3等等，Netscape及新版的IE都支持。url为音频或视频文件及其路径，可以是相对路径或绝对路径。

**2、实例**
```
<embed src="your.mid">
```

### source

**1、定义和用法**

<source> 标签为媒介元素（比如 <video> 和 <audio>）定义媒介资源。
<source> 标签允许您规定可替换的视频/音频文件供浏览器根据它对媒体类型或者编解码器的支持进行选择。

**2、实例**
```
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
 </audio> 
```
### track

**1、定义和用法**

<track> 标签为诸如 video 元素之类的媒介规定外部文本轨道。

用于规定字幕文件或其他包含文本的文件，当媒介播放时，这些文件是可见的。

目前所有主流浏览器都`不支持` <track> 标签。

**2、实例**
```
<video width="320" height="240" controls="controls">
  <source src="forrest_gump.mp4" type="video/mp4" />
  <source src="forrest_gump.ogg" type="video/ogg" />
  <track kind="subtitles" src="subs_chi.srt" srclang="zh" label="Chinese">
  <track kind="subtitles" src="subs_eng.srt" srclang="en" label="English">
</video>
```

### bdi

**1、定义和用法**

bdi 指的是 bidi 隔离。

<bdi> 标签允许您设置一段文本，使其脱离其父元素的文本方向设置。

在发布用户评论或其他您无法完全控制的内容时，该标签很有用。

浏览器支持差。

**2、实例**
```
<ul>
  <li>Username <bdi>Bill</bdi>:80 points</li>
  <li>Username <bdi>Steve</bdi>: 78 points</li>
</ul>
```

### ruby & rp & rb & rt

**1、定义和用法**

<ruby> 标签定义 ruby 注释（中文注音或字符）。

在东亚使用，显示的是东亚字符的发音。

与 <ruby> 以及 <rt> 标签一同使用：

ruby 元素由一个或多个字符（需要一个解释/发音）和一个提供该信息的 rt 元素组成，还包括可选的 rp 元素，定义当浏览器不支持 "ruby" 元素时显示的内容。

<rb> 要注音的对象。

**2、实例**
```
<ruby>
  <rb>千锋教育</rb>
  <rp>(</rp>
  <rt>qian feng jiao yu</rt>
  <rp>)</rp>
</ruby>
```

### video

**1、定义和用法**

`<video>` 标签定义视频，比如电影片段或其他视频流。

**2、实例**
```
<video src="movie.ogg" controls="controls">
您的浏览器不支持 video 标签。
</video>
```

### audio

**1、定义和用法**

`<audio>` 标签定义声音，比如音乐或其他音频流。

**2、实例**

```
<audio src="someaudio.wav">
您的浏览器不支持 audio 标签。
</audio>
```

### canvas

**1、定义和用法**

`<canvas>` 标签定义图形，比如图表和其他图像。
`<canvas>` 标签只是图形容器，您必须使用脚本来绘制图形。

**2、实例**

```
<canvas id="myCanvas"></canvas>

<script type="text/javascript">

var canvas=document.getElementById('myCanvas');
var ctx=canvas.getContext('2d');
ctx.fillStyle='#FF0000';
ctx.fillRect(0,0,80,100);

</script>
```

## embed

## video

## audio

## canvas

## 应用缓存
## WebSQL
## 本地存储
## Canvas
## 文件API
## 地理定位
## 拖放
## history
## 全屏
## 网络状态
## WebWorker
## WebSocket

# CSS3

## CSS3选择器
## CSS3边框
## CSS3背景
## CSS3文本
## CSS3颜色
## CSS3盒模型
## CSS3弹性盒布局模型
## CSS3多列布局
## CSS3渐变
## CSS3变形
## CSS3过渡效果
## CSS3动画

## 媒体查询

## Web字体