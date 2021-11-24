# CSS
掌握CSS的基本语法及其相关理论知识，掌握CSS的几种使用方式

了解CSS预处理器的使用以及其解决的问题

多实践，最终达到具备对原型图1:1的还原能力，差不多就出师了
## 学习资料
### 视屏
* ⭐️ [B站 - 为初学者准备的：CSS 速成](https://www.bilibili.com/video/BV1bW411R7hg?spm_id_from=333.999.0.0)
* [尚硅谷HTML+CSS](https://www.bilibili.com/video/BV1XJ411X7Ud?from=search&seid=15840114647034715222&spm_id_from=333.337.0.0)
* [黑马程序员HTML+CSS](https://www.bilibili.com/video/BV14J4114768?from=search&seid=15840114647034715222&spm_id_from=333.337.0.0)
### 文档
* ⭐️ - [入门：菜鸟教程CSS/CSS3](https://www.runoob.com/css/css-tutorial.html) 语法&能力基础
* ⭐️ - [学习CSS布局](https://zh.learnlayout.com/) 布局基础
* 动画
  * [CSS Animation Rocks: 中文](https://cssanimation.rocks/cn/)
  * [css-animation-101仓库](https://github.com/H-Wakanda/css-animation-101-cn)
  * [css-animation-101-cn：中文](https://h-wakanda.github.io/css-animation-101-cn/)
* 字典&查询语法属性使用
    * [参考手册](http://css.doyoe.com/)
    * [MDN:CSS](https://developer.mozilla.org/zh-CN/docs/Web/CSS)

### 电子书
* [CSS 揭秘](https://www.aliyundrive.com/s/zFS9ki8xwVg)

## 知识点
* ⭐️ 书写样式/HTML使用CSS的几种方法
* ⭐️ CSS基本语法
* ⭐️ 选择器的概念
* ⭐️ 盒模型
* ⭐️ 常用的几种选择器
* ⭐️ 常见CSS单位
* ⭐️ 文本相关属性
* ⭐️ 字体相关属性
* ⭐️ 背景相关属性
* ⭐️ 布局
  * ⭐️ 浮动（float）
  * ⭐️ 定位（position）
  * ⭐️ 弹性布局（flex）
  * ⭐️ 其它常见布局
* ⭐️ 伪类
* ⭐️ 伪选择器
* ⭐️ visible/display/opacity区别
* ⭐️ 水平居中实现方案
* ⭐️ 垂直居中实现方案
* ⭐️ 水平垂直居中实现方案
* ⭐️ 属性的继承
* 样式优先级计算策略
* 层级关系
* 动画
  * 过渡效果
  * 动效
* 常见布局
  * 瀑布流
  * 。。。。
* css预处理器（less、sass、styles。。。。）
  * 任选一个，了解简单用法即可
  * 使用预处理器的优缺点，解决了什么问题
* css变量
* css函数
* 文档流
* BFC
* IFC
* 尺寸单位
  * px
  * em
  * rem
  * rpx
  * vh/wh
* 媒体查询
* 响应式Web
* 。。。
## QA

## 面试考题
### 理论
1. css是否会阻塞页面渲染
2. 如果是，如何解除
3. display:none visible:hidden opacity:0; 三者有何区别?分别有作用?都会有什么副作用
4. 有哪些属性是不可以被继承的，哪些可以被继承
5. 响应式布局是如何实现的
6. 一个div的高度100px是被其内容撑开的，如果为其添加样式height:50px;overflow:hidden，会触发回流重绘吗？如果其先有样式position:absolute，再添加上述样式会触发哪些
7. 文档流有哪几种
8. 脱离普通文档流有哪些方式
9. 什么是BFC 
10. 什么是盒模型
11. position 有哪些属性，分别是什么作用（用于什么场景）
12. 如何实现响应式布局
13. 什么是媒体查询
14. 媒体查询有哪些使用场景
15. 如何书写媒体查询
16. 如何保证h5和pc在显示上的一致性
17. px,rem,em,vw,vh,rpx这些单位分别是什么意思,使用场景是什么
18. 如何实现rem布局
19. 如何实现弹性布局
20. 伪类与伪元素的区别
21. css选择器有哪些
22. 简述一下CSS盒模型，可以手动去改变吗
23. box-sizing的属性有哪些，分别是什么作用
24. 样式优先级怎么计算，样式优先级计算策略
25. 设置样式的方法有哪些
26. display有哪些属性
27. 如何做主题(皮肤)切换
28. css变量如何使用
29. 元素层级关系,如何确定任意两个标签在屏幕上的谁层级更高
30. position值有哪些
31. 隐藏元素的方式有哪些
32. 实现动画的方案有哪些
33. transition和animation的区别
34. 清除浮动的方法有哪些
35. 隐藏页面中某个元素的方法有哪些
36. 常见css函数有哪些
37. 什么是回流，什么是重绘

### 场景/代码
#### 1. css计算规则考查
```html
<div class="app">
    <div>
        <h1>标题</h1>
        <p class="color-blue color-red color-yellow">什么颜色</p>
    </div>
</div>
```
```css
.app p{
    color: black;
}
.app .color-yellow{
    color: yellow;
}

.app .color-red{
    color: red;
}

p.color-color-blue{
    color: blue;
}
```

1. 运行后上面的p标签什么颜色
2. css样式权重如何计算的？
3. 存在冲突时，层叠值（一个元素有多个样式规则）计算规则是怎样的？
 
#### 2. 居中方案考查
```html
<div id="parent">
    <div id="child">child</div>
</div>
```
1. 子元素水平居中的方式有哪些
2. 子元素垂直居中的方式有哪些
3. 子元素垂直居中的方式有哪些

#### 4. 简单响应实现
如果期望实现以下的`div`，该如何书写样式
* 在视口宽度 <=750px展示为长宽都为200px的红色方块
* 在视口宽度 >750px且 <=1400px 时展示为 长宽400px的蓝块
* 在视口宽度 >1400px 是展示为 长宽 600px 的黑色方块

```html
<div class='container'></div>
```
#### 5. 如何实现表格斑马纹
#### 6. 实现一个头部导航的吸顶方案有哪些
#### 7. 主题换肤实现方案(如黑夜模式)

### 布局
#### 1.两列瀑布流布局如何实现
#### 2. 三栏布局实现方案
### 动画/图形
1. 实现一个雪花飘落的动画
2. 实现一个箭头
3. 实现一个圆从左右来回滚动100px的动画
4. 画三角形
5. 画正方体
6. 画梯形
7. 画圆形
8. 画五角星