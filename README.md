# 平时看到的好的知识点博客收集
# 多线程
http://blog.csdn.net/zyplus/article/details/6672775   sleep(),yield(),wait()详解

http://dylanxu.iteye.com/blog/1322066   sleep(),yield(),wait()详解

http://www.importnew.com/14958.html   Java线程中yield与join方法的区别

http://auguslee.iteye.com/blog/1292335    Java Callable用法

http://www.iteye.com/topic/1002652    CountDownLatch用法

http://www.cnblogs.com/cuiliang/p/3327039.html

#单元测试
http://blog.csdn.net/chjttony/article/details/14522771      使用Mock编写java单元测试


#正则
http://www.jb51.net/tools/zhengze.html


#大数据
http://eric-gcm.iteye.com/blog/1807468    hadoop中使用MapReduce编程实例


#分布式
http://www.importnew.com/20344.html   使用 RMI + ZooKeeper 实现远程调用框架


#网站
http://www.importnew.com/

#webservice
http://yufenfei.iteye.com/blog/1685249

#前端
echarts   easyui
http://echarts.baidu.com/examples.html#chart-type-bar
http://blog.sina.com.cn/s/blog_8261811d0102w07r.html
http://www.jeasyui.com/index.php

#spring aop redis
http://blog.csdn.net/zhanngle/article/details/41077423
http://blog.csdn.net/u014695188/article/details/51499947

#网页调用迅雷下载
http://blog.csdn.net/mlianghua/article/details/6025983
http://download.csdn.net/detail/gulu_gulu_jp/9450850

#blog
http://www.cnblogs.com/xdp-gacl/

#Activiti工作流
http://topmanopensource.iteye.com/blog/1315238
http://blog.csdn.net/shirdrn/article/details/6270506
http://wenku.baidu.com/link?url=nYI2l2KQpQIQA3Igr_vHzCUgfyyiWEYmVH8pX4XCUjceWKmzF9kTxy_p66bxybc9ta8WWgpF2nYWpxT-Nusx3WB6Qy9IfTh_MA30VvadZaS
http://www.iteye.com/topic/1134046
http://itindex.net/detail/54221-acitiviti-%E5%9C%A8%E7%BA%BF-%E8%AE%BE%E8%AE%A1/
http://blog.csdn.net/shirdrn/article/details/6271916
http://blog.csdn.net/shirdrn/article/details/6274744
activiti5.18以下只支持Mybatis3.2.5，不支持3.3.0，否则会报SQL错误。
http://www.oschina.net/question/2524100_2141829
http://www.zuidaima.com/share/2186311533595648.htm
http://www.bubuko.com/infodetail-1006099.html
http://www.bug315.com/article/128.htm

#JAVA
http://www.cnblogs.com/xdp-gacl/
http://www.cnblogs.com/ITtangtang/
http://www.zuidaima.com/share/1754065983409152.htm
http://blog.csdn.net/u014695188/article/details/51499947
http://blog.csdn.net/zhanngle/article/details/41077423
http://www.cnblogs.com/yjmyzz/p/4210554.html
http://doc.okbase.net/Naploen8/archive/124775.html
http://blog.csdn.net/qyl445/article/details/9837579
http://www.cnblogs.com/surge/p/3582248.html
http://blog.csdn.net/qiaqia609/article/details/11048463
http://blog.csdn.net/qinpeng100423/article/details/6895978/
http://www.bubuko.com/infodetail-959947.html
http://www.jb51.net/article/77096.htm
http://www.tuicool.com/articles/beUVjyB
http://blog.csdn.net/u014695188/article/details/51488895
http://outofmemory.cn/code-snippet/3025/spring-AOP-Around-Before-After-differentiate
http://www.yiibai.com/spring_mvc/configuring-static-resource-and-resource-bundle-in-spring-mvc.html
http://blog.csdn.net/qzshiyongjie123/article/details/19563249/

#Mysql
http://www.cnblogs.com/huangye-dream/archive/2013/05/30/3108298.html
http://blog.csdn.net/e421083458/article/details/38342051
http://www.jb51.net/article/75451.htm

#interllij 激活码
http://blog.csdn.net/u012400327/article/details/50946103
http://blog.csdn.net/dc_726/article/details/42784275

#JAVA中文乱码
get方式提交中文数据乱码产生的原因和解决办法

对于以get方式传输的数据，request即使设置了以指定的编码接收数据也是无效的(至于为什么无效我也没有弄明白)，默认的还是使用ISO8859-1这个字符编码来接收数据，客户端以UTF-8的编码传输数据到服务器端，而服务器端的request对象使用的是ISO8859-1这个字符编码来接收数据，服务器和客户端沟通的编码不一致因此才会产生中文乱码的。解决办法：在接收到数据后，先获取request对象以ISO8859-1字符编码接收到的原始数据的字节数组，然后通过字节数组以指定的编码构建字符串，解决乱码问题。

post方式提交中文数据乱码产生的原因和解决办法

之所以会产生乱码，就是因为服务器和客户端沟通的编码不一致造成的，因此解决的办法是：在客户端和服务器之间设置一个统一的编码，之后就按照此编码进行数据的传输和接收。
　　由于客户端是以UTF-8字符编码将表单数据传输到服务器端的，因此服务器也需要设置以UTF-8字符编码进行接收，要想完成此操作，服务器可以直接使用从ServletRequest接口继承而来的"setCharacterEncoding(charset)"方法进行统一的编码设置。使用request.setCharacterEncoding("UTF-8");设置服务器以UTF-8的编码接收数据后，此时就不会产生中文乱码问题了。

在Servlet中实现请求转发的两种方式：
　　1、通过ServletContext的getRequestDispatcher(String path)方法，该方法返回一个RequestDispatcher对象，调用这个对象的forward方法可以实现请求转发。
2、通过request对象提供的getRequestDispatcher(String path)方法，该方法返回一个RequestDispatcher对象，调用这个对象的forward方法可以实现请求转发。

请求重定向和请求转发的区别
　　一个web资源收到客户端请求后，通知服务器去调用另外一个web资源进行处理，称之为请求转发/307。
　　一个web资源收到客户端请求后，通知浏览器去访问另外一个web资源进行处理，称之为请求重定向/302。




JS Object拷贝问题，涉及浅拷贝与深拷贝的，可将Object转化成String再赋值，这样两个Object就不互相影响了。
var queryDataStr = JSON.stringify(treeData);
var queryData = JSON.parse(queryDataStr);
