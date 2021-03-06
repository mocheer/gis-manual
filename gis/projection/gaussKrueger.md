#  高斯-克吕格投影
高斯-克吕格投影(gaussKrueger projection)按照投影带中央子午线投影为直线且长度不变和赤道投影为直线的条件，确定函数的形式，从而得到高斯一克吕格投影公式。

投影后，除中央子午线和赤道为直线外，其他子午线均为对称于中央子午线的曲线。设想用一个椭圆柱横切于椭球面上投影带的中央子午线，

按上述投影条件，将中央子午线两侧一定经差范围内的椭球面正形投影于椭圆柱面。将椭圆柱面沿过南北极的母线剪开展平，即为高斯投影平面。取中央子午线与赤道交点的投影为原点，中央子午线的投影为纵坐标x轴，赤道的投影为横坐标y轴，构成高斯克吕格平面直角坐标系。

![](../../assets/18.jpg "GaussKrueger投影示意图")

##  特性
- 等角投影——投影前后的角度相等，但长度和面积有变形。
- 等距投影——投影前后的长度相等，但角度和面积有变形。
- 等积投影——投影前后的面积相等，但角度和长度有变形。

##  特点
- 中央子午线无变形,离中央子午线越远，变形越大。
- 如果中央子午线输错了，投影的中央子午线就会编离实地坐标系正确的中央子午线，变形就越大，测量误差就越大。
- 除中央经线上长度比为1以外，其它任何点长度比均大于1。
- 在同一条纬线上，离中央经线越远则变形越大，最大值位于投影带边缘。
- 在同一条经线上，纬度越低变形越大，最大值位于赤道上。
- 不同的带不能合并，覆盖范围小，适用于小地区的地图，一个带就能覆盖的地区。

##  分带投影
我国3度带共计22带（24～45带）。自1.5度子午线起每隔经差3度自西向东分带，带号依次编为三度带第1、2…120带。 
我国的经度范围西起73°东至135°，可分成六度带十一个，各带中央经线依次为75°、81°、87°、……、117°、123°、129°、135°，或三度带二十二个。

六度带可用于中小比例尺（如1：250000）测图，三度带可用于大比例尺（如1：10000）测图，城建坐标多采用三度带的高斯投影。

1. 高斯投影6度带：自0度子午线起每隔经差自西向东分带，依次编号1,2,3,…60。我国6度带中央子午线的经度，由75度起每隔6度而至135度,共计11带（13～23带），带号用n表示，中央子午线的经度用L表示，它们的关系是L=6n-3。

2. 高斯投影3度带：它的中央子午线一部分同6度带中央子午线重合，一部分同6度带的分界子午线重合，如用n表示3度带的带号，表示L带中央子午线经度，它们的关系L=3n。

##  相关投影坐标系命名方式
- Beijing_1954_3_Degree_GK_CM_75E.prj
- Beijing_1954_3_Degree_GK_Zone_25.prj
- Beijing_1954_GK_Zone_13.prj
- Beijing_1954_GK_Zone_13N.prj
- Xian_1980_3_Degree_GK_Zone_38 

对它们的说明分别如下：
- 三度分带法的北京54坐标系，中央经线在东75度的分带坐标，横坐标前不加带号
- 三度分带法的北京54坐标系，中央经线在东75度的分带坐标，横坐标前加带号
- 六度分带法的北京54坐标系，分带号为13，横坐标前加带号
- 六度分带法的北京54坐标系，分带号为13，横坐标前不加带号
- 三度分带法的西安80坐标系，分带号为38（中央经线为114）

##  自定义独立坐标系
一般来说，很多区域的高斯投影会有自己独立的坐标系

iserver北京超图发布的高斯投影地图接入所需参数：
- falseEasting(东伪偏移)：投影平面中为避免横轴(经度方向)坐标出现负值,而所加的偏移量。如:500000
- falseNorthing(北伪偏移)：投影平面中为避免纵轴(纬度方向)坐标出现负值,而所加的偏移量。如：0
- centralMeridian(中央子午线)
- leftBottom(左下)
- rightTop(右上)