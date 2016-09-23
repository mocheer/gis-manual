# Web墨卡托投影(球形墨卡托投影)
球形墨卡托投影(Spherical Mercator)在Web方面应用最为广泛。

区别:
- 椭球体->圆形球体

参数：
- 球半径：以WGS84椭球的长半轴半径为球半径，即球半径取6378137米。(部门用的Flex地图端测距是6378000米，我认为是不太准确的)
- 赤道周长:2*PI*r = 2*20037508.3427892
- 投影坐标系：以赤道为标准纬线，本初子午线为中央经线，两者交点为坐标原点，向东向北为正，向西向南为负。
- x：[-20037508.3427892,20037508.3427892]
- y：[-20037508.3427892,20037508.3427892]
- lon：[-180,180]
- lat：[-85.05112877980659，85.05112877980659]