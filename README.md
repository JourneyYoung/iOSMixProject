# iOSMixProject
马甲包混淆工程

# 工程目前所具备的功能
1、图片资源修改名字

2、修改工程名

3、类前缀修改，如“GD”修改为“IE”，即修改了文件名

4、混淆随机添加垃圾代码、参数

5、修改方法名前缀

6、人工修改部分方法名，人工对重要类中的方法进行打乱排序

7、(可选)本地图片超轻量级压缩，打乱hash值，新上的马甲包建议修改

#使用方法
先配置启动参数再运行，如图

![image_0](http://ok9lu0v73.bkt.clouddn.com/image.png)
参数解释：

1.工程代码的绝对路径

2.-modifyProjectName [原工程名]>[新工程名]

3.-modifyClassNamePrefix [xcodeproj文件的绝对路径，不是pod安装后的那个打开文件] [旧类前缀]>[新类前缀]

4.-spamCodeOut

5.-ignoreDirNames [需要忽略的文件夹],[需要忽略的文件夹]             注意，Pods文件夹不在混淆范围内，不需要写

6.-handleXcassets              (混淆图片文件)

7.-deleteComments             (删除多余的空格和注释)

8.-chageAPIPrefix [旧方法名前缀]>[新方法名前缀]              注意，前缀要有“_”才能被识别，如果之前工程中没有xx_下划线开头来命名方法的，此项不要勾选

此工程可以选择混淆概率，修改工程中kPercent数值。
#实际测试

![image_1](http://ok9lu0v73.bkt.clouddn.com/i18%5Epimgpsh_fullsize_distr.png)

