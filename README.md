#Color Thief

A script for grabbing the color palette from an image. Uses Javascript and the canvas tag to make it happen.
获取一张图片的整图平均颜色.使用了Canvas标签来实现这个功能。
[See a Demo](http://lokeshdhakar.com/projects/color-thief) | [Read more on my blog](http://lokeshdhakar.com/color-thief)


##How to use

###Get the dominant color from an image

获取一个区域的dominant color(区块平均颜色).
```js
var colorThief = new ColorThief();
colorThief.getColor(sourceImage);
```

```js
getColor(sourceImage[, quality])
returns {r: num, g: num, b: num}
```

###Build a color palette from an image
获取一个图片中的颜色，根据其中的主次来生成一个调色版。
In this example, we build an 8 color palette.
在下面这个例子中，我们从图片对象中获取8个主要的颜色，生成调色器。

```js
var colorThief = new ColorThief();
colorThief.getPalette(sourceImage, 8);
```

```js
getPalette(sourceImage[, colorCount, quality])
returns [ [num, num, num], [num, num, num], ... ]
```


## My Changelog
This is a fork from [lokesh/color-thief](http://lokeshdhakar.com/projects/color-thief), which devote to adding more interfaces .

V1.0.1 添加中文文档
