## 1.	关于这次我写的个人网站，概况如下。

   首先对于整个界面的大致架构，我采用了3个div盒子来完成，第一部分用于显示整个网页上面的图片，第二个用于显示导航栏，第三个内部设有一个iframe框架作为target窗口显示导航栏各部分的详细内容，这样就省掉了新打开窗口或者再度返回的麻烦，整个网站也就更加的简约，全部都采用sublime编辑器写的。
   接下来说一下各个部分的大致内容：

### --自我介绍页

   整个自我介绍我都采用了一个框架结构，上列是大标题与背景，左边是一个纵向显示的列表，右边部分则是显示各分项的详细信息。但是其中大部分类容都是从网上引用过来，整个自我介绍页都是在html初学时写的，运用的东西也都比较基础，包括字体的设置，框架的运用等。

### --相册页

   在相册里面，我在htmleaf上引用了一个js脚本，同时对其中一些原网站中的不必要的东西加以删改，以适应我的网页的的布局。但是由于这个效果是由js与css相结合做出来的，所以修改的过程非常非常的麻烦，先是把所有的css文件都看了一遍，把所有的架构全部弄清楚之后再逐个进行修改、调试，而且，某些图片效果的显示会与之前所设好的框架不协调，又得自己去酌情地改变某些属性以达到最佳浏览效果。

### --心情日记页

   这个界面是我借鉴了一个网站的的风格而做的，每一个日记都是由3个div盒子再配合各种浮动，边距，hover等配合达到一种朦胧又能够突出的比较精致的效果。

### --联系页面

   在联系页面里我用了两个链接打开电脑本地的QQ与邮箱用以联系我。
对于整个网页的一些很细节方面的修饰，比如一些盒子的阴影，边角弧度，和hover效果等，也使得网页更加美观，网站所有的照片都是自己从网上下载，经过自己P图或者调整大小后，再转入网易相册，再将地址复制而得到的，而后各个网页都是由自己的超链接。


## 2.	具体的实现：

   整个大框架主要都是由nav盒子的ul导航栏作为中转，将每一个li与a都加上display: block使其变为块级元素，然后再令其全部向左浮动以达到横向分布效果，并且设置list-style-type: 去掉\<li>的圆点，对于每一个\<li>都给链入对应的html文件并显示到name为down的iframe中。
自我介绍页我主要采取了教材上老式的frameset来作为框架，分为上、左、右三个frame，分别设好name并调节好cols与rows属性，左列的导航栏设了较大的line-height值与字体来突出效果，对\<ul>的每一个\<li>都设有一个超链接指向对应的网页，个人信息采用表格的形式，对于照片及对自己的评价语段等占空间多的\<td>都给设rowspan来调节，自我介绍的标题则是用div居中+背景图片+文字来完成，其中工作经验和自我评价是从网上摘抄。
我的相册部分是从htmleaf站点中一篇有着5个js效果的文章上将源代码下载，之后有与只想引用其中的一个，而目前对js效果的各种用法与语法并不熟悉，便只是从对应的css盒子中去掉了对其余四个效果的引用语句，接而将原网页中赘余的文字段落，链接和其他一些不需要的效果也去掉，并且细读了它与js脚本配合的生成动态效果的各个css文件，对齐div的各种属性进行删改，以达到自己想要的效果。
至于心情日记这一部分则是在div的浮动的同时运用一些小小的css效果，如box-shadow与hover、color相配合从而实现了每一篇文字都如同3D一般的效果，再加上调节边距，找文字图片素材等实现其布局和内容。
联系方式这一页除了写了个电话号码，下面就是链入了QQ的协议地址tencent://message/?uin直接与我的QQ发消息，并且另外链入了邮箱地址mailto以在当前计算机直接打开电子邮箱的客户端软件给我发邮件。


## 3.	待改进的地方：
   这一次的网站由于我自己对知识掌握得不够熟练，再加上完成得匆忙，导致如屏幕适应，和兼容性等等很多地方可能都还有不足，还有一些想做的东西也还没做上，如我想在边上加上类似于分享到QQ空间或微博的浮标，再网页打开时加入一个欢迎效果作为一个引入界面，最上方的图片制作成能够链入不同界面的轮播图，再给网页加入背景音乐等等。
   以后随着我的技能提升，我会慢慢的一点点修改和完善，争取将这个网站做得真正有模有样。
  <a href="https://zz13372410754.github.io/fourth/mysite/homepage.html">网址</a>
