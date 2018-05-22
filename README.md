# shell-mysql
使用shell脚本分页读取MySQL数据

###脚本背景
**由于要在Linux上，远程读取mysql的表的数据，然后做一定清洗后，把数据上传至Hadoop集群中，使用Java写吧，感觉太麻烦了，得在Win上开发好，还得打成jar包，
上传到Linux上，如果那里出了问题，还得重复这样，非常不方便，那就用shell写一个吧，也不需要什么jdbc驱动包，只需要在Linux上装个MySQL的
客户端即可，用一行yum命令即可搞定，所以就花了点时间，封装了一个小脚本**

###功能介绍
**直接在Linux下使用shell脚本远程分页读取MySQL表的数据的一个小脚本，已测过读取600万+的数据
效率与jdbc相差无几**

###脚本介绍
**主要有三个脚本构成<br/>1，page.sh 这是一主脚本，里面定义了分页的条件，大家看下便知<br/>2，f.sh   一个小包装的脚本吧，里面会用sed去掉表头一些信息<br/>3，port.sh  分页读取数据的执行脚本<br/>**


###如何使用？
**使用非常简单，需要改下page.sh里面的查询字段，以及分页查询的数量，默认是10000，然后执行sh page.sh databaseName tableName传入数据库名和表名即可**

## 博客相关

（1）[微信公众号（woshigcs）：同步更新](https://github.com/qindongliang/answer_sheet_scan/blob/master/imgs/gcs.jpg)

（2）[个人站点(2018之后，同步更新）](http://8090nixi.com/) 

（3）[腾讯云社区，自动同步公众号文章](<http://qindongliang.iteye.com/>)

（4）[csdn ： (暂时同步更新)](https://blog.csdn.net/u010454030)

（5）[iteye（2018.05月之前所有的文章，之后弃用）](<http://qindongliang.iteye.com/>)  






## 我的公众号(woshigcs)

有问题可关注我的公众号留言咨询

![image](https://github.com/qindongliang/answer_sheet_scan/blob/master/imgs/gcs.jpg)
