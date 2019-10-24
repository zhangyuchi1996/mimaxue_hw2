使用GmSSL和ImageMagick对pku logo进行加密<br>
加密的图片如下：<br>
![](https://github.com/zhangyuchi1996/mimaxue_hw2/blob/master/logo/logo.jpg)
<br>步骤如下：<br>
1、使用IamgeMagick将图片转化为rgba格式<br>
convert -depth 8 logo.jpg logo.rgba<br><br>
2、使用gmssl的ecb模式和cbc模式分别将图片加密<br>
gmssl enc -sms4-ecb -e -in logo.rgba -out logo_ecb.rgba<br><br>
gmssl enc -sms4-ecb -e -in logo.rgba -out logo_cbc.rgba<br><br>
3、使用ImageMagick将加密后的文件转化为图片<br>
convert -size 720x720 -depth 8 logo_ecb.rgba logo_ecb.jpg<br><br>
convert -size 720x720 -depth 8 logo_cbc.rgba logo_cbc.jpg<br><br>
效果如下：<br>
![](https://github.com/zhangyuchi1996/mimaxue_hw2/blob/master/logo/logo_cbc.jpg)
![](https://github.com/zhangyuchi1996/mimaxue_hw2/blob/master/logo/logo_ecb.jpg)
