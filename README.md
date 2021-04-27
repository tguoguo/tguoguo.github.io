# tguoguo.github.io
# 计算机科学与编程入门课程第二次作业
##  2010301336 唐果菓

## 作业一：词频统计图
对于已有的小说《当呼吸化为空气》的人物词语频数csv文件，通过柱状图、词云图和饼状图三种方式来实现了词频的可视化。在三个可视化的做法中首先通过相同的分词操作将人物和词频分为两个列表。
在柱状图中运用了最基本的柱状图格式并改变了标题的样式；在词云图中将词云设置为三角形，改变了词语和标题的字体并自己设置了布局和大小，在饼状图中采用了空心的南丁格尔玫瑰图，加入了工具箱配置项，并且将图例改为了棱形。
三个图均将标题放在了正中间，并采用了相应的themetype。

[作业一链接]（https://tguoguo.github.io/柱状图.html ）
          （https://tguoguo.github.io/词云图.html ）
          （https://tguoguo.github.io/饼状图.html ）

## 作业二：地理连线图
故事背景：一群复生会的教徒们最近开始活跃起来，因为30天以后将会是复生会的复生日，为了迎接真神的降临，他们必须在地图上燃起4组代表复生的火把，每一组的4个火把放置的地点必须构成交叉的十字，真神就会降临在这4组火把中心的位置。

操作：采用geo以中国地图为背景，通过json的方式向其中添加了16个点的位置，通过瞄点连线将每组的四个火把连接成为交叉的十字，瞄点采用了scatter和effect_scatter两种方式分别标注火把位置和真神降临位置，并设置了themetype

[作业二链接]（https://tguoguo.github.io/地理连线图.html ）

## 作业三：中国地图&世界地图
故事背景：从小居住在重庆的小唐最近十分焦虑，因为她还不知道如何填报自己的高考志愿。小唐从小对于温度十分敏感，所以她十分看重城市气候是否宜人，她需要先了解她心仪的几个城市每个月的平均最高温度和最低温度，作为填报志愿重要的参考。

操作：选择了中国地图作为背景，结合timeline的形式用两个series标出了全国北京、上海等14个省市每个月的平均最高气温和最低气温。考虑到系统自动设置的温度区间划分方式每个区间过大，故手动设置了每个区间的值使得visual的对比度更强。

[作业三链接]（https://tguoguo.github.io/中国地图.html ）

## 作业四：组合图表
故事背景：作为坐拥亿万资产的富豪唐大富，在新冠肺炎疫情肆虐全球的危急情况下，老唐觉得自己应该积极运用自己的资产做慈善。老唐和朋友们一起购置了一大批呼吸机发往世界各地，她被分配到的区域是印度，现在她需要了解印度各地现存的确诊病例数,危重症病人比例以及现有的呼吸机数，来分配寄到印度各地的呼吸机数目。



操作：通过grid的方式将map和bar组合到一起，通过url将印度的地图导入，用map表示印度各地区现有的呼吸机数目。因为地区的数据较多，所以采用了zoom的效果并结合了inside效果使得更易进行横向比较。同时危重症和普通病例的比例也对于判断有影响，所以采用stack的方式进行堆叠。

[作业四链接]（https://tguoguo.github.io/组合图表.html ）



# 计算机科学与编程入门课程第三次作业
##  2010301336 唐果菓

## 作业一：人物关系图
选择了小说《德伯家的苔丝》进行人物关系图的分析，考虑到小说中的段落划分并非中国古典小说一大段为一段对话，而是一个人物的一句话就是一个段落，故采用了分章节进行人物共现判断，判断标志为换行+下一行的第一个字符为数字。同时检查了小说内容，除了章节的开头为数字之外，无其他段落开头为数字。因为章节较段落更加长，导致共现次数过大，所以在用共现次数绘制graph时设置了限制值为1000。在统计人物以及出现次数时同样根据内容设置了相应的限制值。在绘制graph时，同时采用了circular和force两种方式，对比起来force经过repusion等值的调节仍然会导致点的重叠，看起来更乱，circular则不会，但是人物亲疏关系表现得不如force，两者相互补充。在circular对人物进行了分类，使得对比更加鲜明，方便分类查看，考虑到force图已经够乱了，故没有采用分类。

[作业一链接]（ https://tguoguo.github.io/《德伯家的苔丝》circular.html ）
                   (https://tguoguo.github.io/《德伯家的苔丝》force.html)

## 作业二：搜索引擎
使用html编写了名为“这是一个搜索引擎“的搜索引擎，页面主要有以下几个部分：标志，题目，搜索框，搜索按钮，今日热搜。在标志部分加入了一个动图；搜索框设置了背景图片，提示语，边框的颜色，以及点击搜索框时加上了边框的动态变化效果。按钮采用了bootstrap中的按钮样式，点击后会跳转至百度搜索；在页面下方设计了一个今日热搜板块，采用table的方式列出了前五条热搜，题目上有超链接可点击跳转，在后边加上了相应的表情来美化。最后通过div分区的方式设置相应的位置实现了整体的布局。

[作业二链接]( https://tguoguo.github.io/searching.html )

##作业三：四大医学期刊
网页标题为四大医学期刊，主要介绍了医学领域的四大顶级期刊:the lancet, BMJ, JAMA, NEJM。主要有标题，主页面，更多期刊板块和页面导航卡片。



标题位于页面的右上方，设置了背景和文字颜色，同时通过padding等设置将字放在了中间。



主要内容部分整体也位于页面的右方，在导入语的部分通过iframe展示了四大期刊的封面。之后的每一个期刊包含标题、图标、简介、主页链接和近期学术热点几项内容。除了设置文字的样式外，将图片float在文字右边，主页和每一篇新文章都有相应的超链接，可以直接点击进入。



在更多期刊部分采用了bootstrap中的卡片样式，插入了相应的图片和期刊名称来展示更多的六种期刊，同时每一个期刊的名称都设置有超链接，可以通过直接点击的方式访问期刊的主页。



在页面的右边设置了页面导航，采用了bootstrap中的卡片样式，将卡片位置始终固定在页面的左边，通过id索引的方式点击标题实现页面的导航。但存在的问题是导航卡片会遮挡期刊的图片，本来设想通过collapse折叠的方式将导航卡片藏起来，但是经过了多次尝试后还是未能实现。



最终通过设置div分区的位置达到整体的布局。
[作业三链接] （ https://tguoguo.github.io/四大期刊.html ）
