# study-CSS3
learn CSS3



一、新增选择器
 1、字符串匹配属性
  ①、完全匹配：元素[属性="值"]
  ②、匹配开头：元素[属性^="值"]
  ③、匹配结尾：元素[属性$="值"]
  ④、包含：元素[属性*="值"]
 2、目标伪类
  ①、:checked
  ②、:selected
  ③、:disabled
  ④、::selection
 3、结构性伪类选择器
  ①、:nth-child(n)
  ②、:nth-of-type(n)
 4、兄弟选择器：在同一级上
  ①、+
  ②、~
 5、子元素选择器
  ①、>
 6、伪元素选择器
  ①、:before
  ②、:after
 7、:not()
二、transition过渡
 原理: 从初始状态到结束状态，过渡属性加在结束状态
 transition: 参与过渡的属性  过渡时间  过渡动画类型  延迟时间
 多个属性需要参与过渡，写一个transition, 里面的值以逗号分开
三、@media媒体查询器
目的：实现响应式布局
原理: 根据当前所使用的设备窗口分辨率，决定调用哪一套CSS样式
CSS: @media (max-width="1200px"){}
四、font字体
字体图标的好处：文档小，是矢量、随时改变颜色
导入文档字体：@font-face{	font-family:"自定义字体名称";	src:url("字体文档路径");} 应用字体：font-family:"自定义字体名称";
五、animation动画
 定义动画规则：@-webkit-keyframes 规则名称{	from{}	to{}}@-webkit-keyframes 规则名称{	0%{}	100%{}} 调用动画：animation: 动画规则名称 持续时间 过渡类型 延迟时间 循环次数(infinite) 结束停留状态(forwards) 运动方向(alternate)
六、transform变换
 translate() 平移、scale() 放大缩小、skew() 扭曲、rotate() 2D旋转、rotateX()/rotateY() 3D旋转、matrix() 矩阵
七、shadow阴影
 box-shadow：1.X轴偏移 2.Y轴偏移 3.模糊值 4.外延值 5.颜色 6.内阴影inset；例如：box-shadow:15px 15px 10px 0px red,30px 30px 10px 0px yellow;
 text-shadow：1.X轴偏移 2.Y轴偏移 3.模糊值 4.颜色
八、border边框
 圆角border-radius：Xpx（一个值）、左上右下  右上左下（两个值）、左上  右上左下  右下（三个值）、左上  右上 右下 左下（四个值）
 border-image：不推荐使用，一个字，丑
九、颜色
 透明度rgba(0-255,0-255,0-255,0-1)，数字越大透明度越低
 opacity: 0-1
 区别：
 Opacity:整个元素包含的内容全部透明，opacity是一个属性
 RGBA: 只针对于当前的属性进行颜色透明化，RGBA是一个颜色值
