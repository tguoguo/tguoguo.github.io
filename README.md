# tguoguo.github.io
# 计算机科学与编程入门课程第二次作业
##  2010301336 唐果菓

## 作业一：词频统计图
对于已有的小说《当呼吸化为空气》的人物词语频数csv文件，通过柱状图、词云图和饼状图三种方式来实现了词频的可视化。在三个可视化的做法中首先通过相同的分词操作将人物和词频分为两个列表。
在柱状图中运用了最基本的柱状图格式并改变了标题的样式；在词云图中将词云设置为三角形，改变了词语和标题的字体并自己设置了布局和大小，在饼状图中采用了空心的南丁格尔玫瑰图，加入了工具箱配置项，并且将图例改为了棱形。
三个图均将标题放在了正中间，并采用了相应的themetype。

[作业一链接]（https://tguoguo.github.io/柱状图.html）
          （https://tguoguo.github.io/词云图.html）
          （https://tguoguo.github.io/饼状图.html）

##作业二：地理连线图
故事背景：一群复生会的教徒们最近开始活跃起来，因为30天以后将会是复生会的复生日，为了迎接真神的降临，他们必须在地图上燃起4组代表复生的火把，每一组的4个火把放置的地点必须构成交叉的十字，真神就会降临在这4组火把中心的位置。
操作：采用geo以中国地图为背景，通过json的方式向其中添加了16各点的位置，通过瞄点连线将每组的四个火把连接成为交叉的十字，瞄点采用了scatter和effect_scatter两种方式分别标注火把位置和真神降临位置，并设置了themetype

[作业二链接]（https://tguoguo.github.io/地理连线图.html）

##作业三：中国地图&世界地图
故事背景：从小居住在重庆的小唐最近十分焦虑，因为她还不知道如何填报自己的高考志愿。小唐从小对于温度十分敏感，所以她十分看重城市气候是否宜人，她需要先了解她心仪的几个城市每个月的平均最高温度和最低温度，作为填报志愿重要的参考。
操作：选择了中国地图作为北京，结合timeline的形式用两个series标出了全国北京、上海等14个省市每个月的平均最高气温和最低气温。考虑到系统自动设置的温度区间划分方式每个区间过大，故手动设置了每个区间的值使得visual的对比度更强。

[作业三链接]（https://tguoguo.github.io/中国地图.html）

##作业四：组合图表
故事背景：作为坐拥亿万资产的富豪唐大富，在新冠肺炎疫情肆虐全国的危急情况下，老唐觉得自己应该积极运用自己的资产做慈善。老唐和朋友约好一起购置了一大批呼吸机发往世界各地，她被分配到的区域是印度，现在她需要了解印度各地现存的确诊病例数,危重症病人比例以及现有的呼吸机数，来分配寄到印度各地的呼吸机数目。
通过grid的方式将map和bar组合到一起，通过url将印度的地图导入，用map表示印度各地区现有的呼吸机数目。因为地区的数据较多，所以采用了zoom的效果并结合了inside效果使得更易进行横向比较。同时危重症和普通病例的比例也对于判断有影响，所以采用stack的方式进行堆叠。

[作业四链接]（https://tguoguo.github.io/组合图表.html）
