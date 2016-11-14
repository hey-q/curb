# curb
curb是一个导航页,目前由hey-q团队维护，发布重要工具类链接。



## tinypng
一个好用的图片压缩工具。如下图所示，可以在不改变图片尺寸，且对清晰度影响不大的前提下，把一张496.1K的图片压缩到33K.

访问地址 [https://tinypng.com](https://tinypng.com)

需要注意的是图片不要大于5M，我也不知道大于5M的时候会出现什么

![image](./images/tinypng1.png)

## alexa
一个世界范围内的互联网评估工具，专门发布网站排名。适用于产品经理做市场分析

访问地址 [http://www.alexa.com](http://www.alexa.com/)

## coolors
一个色彩搭配方案选择工具，使用空格键切换，免费又好用。适用于设计人员快速找到适用于屏幕显示的一组相互搭配的色彩。

访问地址 [https://coolors.co](https://coolors.co/)

## doyoudo
视频教学网站，开设平面设计、动画、特效制作、音乐音效等课程。大部分课程免费。课程质量相对优秀。

访问地址 [http://doyoudo.com](http://doyoudo.com/)

## atom
一个优秀的免费文档编辑器，由GitHub推出。拥有良好的插件生态。官方提供的markdown插件很好用。号称A hackable text editor for the 21st Century

下载地址 [https://atom.io](https://atom.io/)

## emojione
一个emoji的多端解决方案。emoji编码存储数据库时需要复杂的格式转换，这是一个困扰开发者的难题。emojione提供了两个方法，可以通过引入emojione这个库，把emoji字符转换成字符串，也可以把字符串重新转换成emoji的unicode.

示例代码：
```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>emojione</title>
  <!-- Emoji One JS -->
  <script src="http://cdn.jsdelivr.net/emojione/2.2.6/lib/js/emojione.min.js"></script>
</head>
<body>   
      <div>
        <h3>Input:</h3>
        <input type="text" id="inputText-1" name="inputText-1" size="50" value="Hello world! &#x1f604;"/>
        <input type="button" value="Convert" onclick="convert1()"/>
      </div>
      <div>
        <h3>Output:</h3>
        <p id="outputText-1"></p>
        <script type="text/javascript">
          function convert1() {
            var input1 = document.getElementById('inputText-1').value;
            var output1 = emojione.toShort(input1);
            document.getElementById('outputText-1').innerHTML = output1;
          }
        </script>
      </div>

          <div>
              <h3>Input:</h3>
              <input type="text" id="inputText-2" name="inputText" value="Hello world! :smile:"/>
              <input type="button" value="Convert" onclick="convert2()"/>
          </div>
          <div>
              <h3>Output:</h3>
              <p id="outputText-2"></p>
              <script type="text/javascript">
                  function convert2() {
                      var input2 = document.getElementById('inputText-2').value;
                      var output2 = emojione.shortnameToUnicode(input2);
                      document.getElementById('outputText-2').innerHTML = output2;
                  }
              </script>
          </div>

</body>
</html>
```
项目主页：[http://emojione.com/](http://emojione.com/)

示例页面：[demo](http://119.29.238.25/jstoshort1.html)

emojione是一个很大的项目，做的事情不仅仅是上述转换，也不止包含js的代码，有余力的话可以多研究一下。
