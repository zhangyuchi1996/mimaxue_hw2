使用GmSSL和ImageMagick对pku logo进行加密<br>
加密的图片如下：<br>
![](https://github.com/zhangyuchi1996/mimaxue_hw2/blob/master/logo/logo.jpg)
<br>步骤如下：<br>
1、使用IamgeMagick将图片转化为rgba格式<br>
2、使用gmssl的ecb模式和cbc模式分别将图片加密<br>
3、使用ImageMagick将加密后的文件转化为图片<br>
效果如下：<br>
![](https://github.com/zhangyuchi1996/mimaxue_hw2/blob/master/logo/logo_cbc.jpg)
![](https://github.com/zhangyuchi1996/mimaxue_hw2/blob/master/logo/logo_ecb.jpg)
