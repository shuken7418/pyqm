# python期末项目之The Harm Of Smoking

## github说明及pythonanywhere部署
* [github说明](https://github.com/shuken7418/pyqm)
* [pythonanywhere部署](http://shuken7418.pythonanywhere.com/)

## github包含多少url
* 本项目网站包含7个rul分别为：<br>
[首页/死亡因素词云图](http://shuken7418.pythonanywhere.com/)<br>
[危险因素死亡图](http://shuken7418.pythonanywhere.com/wx)<br>
[因吸烟死亡人数图](http://shuken7418.pythonanywhere.com/yx)<br>
[因吸烟死亡比例图](http://)<br>
[吸烟导致癌症死亡比例图](http://shuken7418.pythonanywhere.com/xy)<br>
[按年龄划分吸烟死亡人数图](http://shuken7418.pythonanywhere.com/nl)<br>
[结论&总结](http://shuken7418.pythonanywhere.com/result)

## html档描述
* [首页/死亡因素词云图](http://shuken7418.pythonanywhere.com/) 展示的是会导致死亡的危险因素，我们可以看到Smoking的出现频率很高。现如今，吸烟已成为危害身体健康的一大危险因素。世界上每年都有几百万人因为吸烟导致死亡，据不完全统计，20世纪因吸烟导致死亡的人数大约有1亿。本项目通过一系列可视化图表，展示吸烟的危害；<br><br>
这些数据的来源是：<br>
International Mortality and Smoking Statistics（IMASS）<br>
Institute of Health Metrics and Evaluation (IHME), Global Burden of Disease (GBD)<br>
World Health Organization (WHO) Global Health Observatory (GHO)

* [危险因素死亡图](http://shuken7418.pythonanywhere.com/wx) 可以看出中国每年有超过200万人因为吸烟死亡;吸烟在世界上是导致死亡的一大危险因素，吸烟会导致肺癌等疾病，严重危害我们的身体健康。在图表中，我们能看到他是中国第二大死亡风险因素;从图表中我们还能看到因为吸二手烟死亡的人数竟高达38万，二手烟对身体健康也会产生严重的危害;

* [因吸烟死亡人数图](http://shuken7418.pythonanywhere.com/yx) 展示的是世界各国因吸烟死亡人数，衡量标准为每个国家每10万人中因吸烟死亡的人数;从地图可以看出，亚洲和东欧国家每年因吸烟死亡人数普遍高于其他国家，死亡人数通常超过100;在一些人均收入较低的国家，吸烟率较低，因此因吸烟死亡率也普遍低于其他高收入国家;

* [因吸烟死亡比例图](http://)

* [吸烟导致癌症死亡比例图](http://shuken7418.pythonanywhere.com/xy) 可以看出全球超过五分之一的癌症死亡是吸烟导致的;美国，加拿大等发达国家吸烟导致癌症死亡比例普遍较高;而一些较为落后的国家，吸烟导致的癌症死亡比例较低;

* [按年龄划分吸烟死亡人数图](http://shuken7418.pythonanywhere.com/nl) 描述的为2000年到2017年中国按年龄划分的吸烟死亡人数（15岁以下人群吸烟死亡数为0，因此不包括15岁以下人群）;从可视化图表可以看出吸烟死亡在老年人口中较为常见，70岁以上占了一半，年轻人和儿童因吸烟死亡人数很低；

* [结论&总结](http://shuken7418.pythonanywhere.com/result) 总结了以上图表得出的数据，得出结论为：<br>
 **为了自己与身边人的健康，请不要吸烟！** 

## Python档描述

* 首先导入render_template函数；
* 引入模块，主要为pyecharts包括pyecharts.charts中的Line,Map,Timeline,Pie, WordCloud还有pandas，options；
* 读取csv数据
* 创建一个新的URL例如'/'
* 创建一个函数返回正确呈现的HTML
* 让web应用开始运行

## HTML5控件

* 在每个html页面（除最后一页）添加了“下一页”的控件

```
    <form method="GET" action="/wx">
<p><input value="下一页更精彩哦 !" type="SUBMIT" ></p>
</form>
```

* 在每个页面添加了导航栏

```
<div class="nav">
<ul>
<li><a href="/">首页</a></li>
<li><a href="/wx">危险因素死亡</a></li>
<li><a href="/yx">因吸烟死亡人数</a></li>
<li><a href="/bl">因吸烟死亡比例</a></li>
<li><a href="/xy">吸烟导致癌症死亡比例</a></li>
<li><a href="/nl">按年龄划分吸烟死亡人数</a></li>
<li><a href="/result">结论&总结</a></li>
</ul>
</div>
```

## 数据交互
* 实现数据的python——>HTML页面交互,(前端能接收到同样的数据传递结果）；
* 含有复杂数据结构的循环；
* 含有合适的数据结构嵌套；
* 含有合适的推导式
* 含有适当的条件判断；
* 函数和模块符合python PEP8标准；
* 符合jinja2标准；
* 上传pythonanywhere，即为[The Harm Of Smoking](http://shuken7418.pythonanywhere.com/)

## 功能具有可扩展和丰富性

* 添加网页背景色，加入css文件中，再由每个html档链接进去；
* 为导航栏添加css样式，其中包括颜色，大小，居中，下边框样式，盒阴影；
* 等等

