# Aakian-FaCai
专门针对前端vue框架的JavaFx图形化GUI漏洞扫描工具，支持一键扫描vue-manage-system系统前端泄露的未授权目录接口漏洞，并且对扫描的暴露目录进行逐一测试和验证，方便渗透人员快速确定未授权接口。还添加了出口IP地址信息本地DNS信息等的查询，方便清楚自身出口IP。

很多人不清楚不了解这个漏洞，所以特地更新了一篇教学文章，https://blog.csdn.net/weixin_43847838/article/details/125841581?spm=1001.2014.3001.5501
欢迎指点。

## 2023年8月10日-> FaCai_V1.0.0_jdk8_zangcc深情版
更换界面GUI

<img src="https://github-production-user-asset-6210df.s3.amazonaws.com/64825932/259633469-a3fdd94a-89af-466c-bcf9-f8e8a6d461f8.png" width="700px">
新增功能：
1、可以自查JS文件。
2、可以自定义URL进行所有接口的拼接测试。

详情可以看教程文章第四大点-（四、2023年8月10日更新内容）：https://blog.csdn.net/weixin_43847838/article/details/125841581?spm=1001.2014.3001.5501



## 2022年6月21日-> Aakian-v1.0
初始版本，功能比较简单，但是也能满足vue的常规扫描。
基于jdk1.8开发，也就是java8，其他版本的jdk可能会无法运行，建议切换到开发版本。
### 工具运行方法：
把xjar.exe文件和Aakian.jar文件放在同一目录下，用下面的命令运行即可。（jdk1.8）


xjar.exe java -jar Aakian.jar

<img src="https://user-images.githubusercontent.com/64825932/174664693-d9eab2cf-1049-43b2-ad0b-f87bd5a23791.png" width="700px">
输入上述命令后即可运行工具，如图所示：

<img src="https://user-images.githubusercontent.com/64825932/174665018-853ba6f4-8a02-40af-b409-5425b1c821c7.png" width="650px">

正常扫描的结果：

<img src="https://user-images.githubusercontent.com/64825932/174708944-700cef67-7a71-46a2-9441-4b0f8e1ab82e.png" width="650px">


### 功能介绍：
扫描vue框架（vue-manage-system）前台泄露的未授权目录接口。
支持所有的接口，并且对接口进行逐一的测试访问。
为了方便验证，返回的是响应包的大小，如果大小类似，说明不存在未授权，接口访问过去返回的还是原来的前台登录界面。
所以也增加了返回包的内容，通过内容，大小，更直观的判断是否页面成功跳转。
### 工具的功能图片&展示：
<img src="https://user-images.githubusercontent.com/64825932/174708944-700cef67-7a71-46a2-9441-4b0f8e1ab82e.png" width="650px">
<img src="https://user-images.githubusercontent.com/64825932/174709151-8d0b105d-0966-4a96-8ea3-3740216da1d8.png" width="650px">


