# Two.js
>一、概述
1、Two.js 简介
    - Two.js 是一个面向现代 Web 浏览器提供绘制二维图形的 API ，它允许使用不同的上下文，而使用相同的 API 进行绘制
    - Two.js 所支持的上下文:
  - SVG
  - Canvas
  - WebGL
  - 官方地址: http://jonobr1.github.io/two.js/

2、Two.js 特点
  - 专注于矢量图:
  - Two.js 是深度实现具有动画效果的矢量图
  - Two.js 致力于更简洁地创建矢量图及动画效果
  - Two.js 不支持文本或图片
  - 场景:
  - Two.js 的核心是依赖于场景
  - 当创建或绘制一个对象 (Two,Polygon 或 Two.Group)时，是同时存储并记忆
  - 循环动画:
  - Two.js 具有一个内置的循环动画
  - Two.js 的动画效果可以很简单的实现，也可以与其他动画库配置使用
  - SVG 解释器:
  - Two.js 具有 SVG 解释器
  - Two.js 允许开发者或设计者在商业应用中创建 SVG，例如使用 Adobe Illustrator 创建的 SVG 元素纳入 Two.js 的场景中

二、Two.js入门
1、Two.js 框架的使用
  - 在 HTML 页面引入 Two.js 文件:
  <script src="two.js"></script>
  - 在 HTML 页面定义用于显示矢量图的容器:
  <div id="draw-shapes"></div>
  - javascript 代码获取元素:
  document.getElementById("draw-shapes");
  - 使用 Two.js 提供的 API 进行绘制
  new Two(params).appendTo(elem);

2、绘制矩形元素
  - Two.js 框架使用makeRectangle(x,y,width,height)方法绘制矩形
  makeRectangle(x,y,width,height)
  - x:指定绘制的矩形左上角的坐标值x
  - y:指定绘制的矩形左上角的坐标值y
  - width:指定绘制的矩形的宽度
  - height:指定绘制矩形的高度
  - Two.js 框架使用makeCircle(x,y,radius)方法绘制圆形:
  makeCircle(x,y,radius)
  - x: 指定绘制圆形的圆心的坐标值x
  - y: 指定绘制圆形的圆心的坐标值y
  - radius: 指定绘制的圆形的半径

3、元素分组
  - 通过 Two.js 框架允许将绘制在页面的多个图形分为一组或多组
  - 通过 Two.js 提供的 API 方法允许针对组进行操作或实现动画
  - 创建分组:
  - 通过 Two.js 框架提供的构造器 Two.Group() 实现
  - 通过 Two.js 提供提供的相关 API 方法或属性进行操作
  - 将已绘制的图形分为一组或多组:
  - 通过创建的two对象调用makeGroup()方法
  - makeGroup() 方法允许传递多个绘制图形对象
  - 通过 Two.js 框架提供的相关 API 方法或属性进行操作

4、添加动画
  - two.play()方法:
  - 该方法向 requestAnimationFrame loop 添加一个实例，使该实例实现动画效果
  - two.pause()方法:
  - 该方法从 requestAnimationFrame loop 删除一个示例，使该示例的动画效果停止
  - two.update()方法:
  - 该方法用于更新在HTML页面中绘制的图形的尺寸，增加动画效果
