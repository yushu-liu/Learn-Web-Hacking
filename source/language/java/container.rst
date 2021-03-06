容器
========================================

常见的Java服务器有Tomcat、Weblogic、JBoss、GlassFish、Jetty、Resin、IBM Websphere等，这里对部分框架做一个简单的说明。

Tomcat
----------------------------------------
Tomcat是一个轻量级应用服务器，在中小型系统和并发访问用户不是很多的场合下被普遍使用，用于开发和调试JSP程序。

在收到请求后，Tomcat的处理流程如下：

- 客户端访问Web服务器，发送HTTP请求
- Web服务器接收到请求后，传递给Servlet容器
- Servlet容器加载Servlet，产生Servlet实例后，向其传递表示请求和响应的对象
- Servlet实例使用请求对象得到客户端的请求信息，然后进行相应的处理
- Servlet实例将处理结果通过响应对象发送回客户端，容器负责确保响应正确送出，同时将控制返回给Web服务器

Tomcat服务器是由一系列可配置的组件构成的，其中核心组件是Catalina Servlet容器，它是所有其他Tomcat组件的顶层容器。

相关CVE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
- `CVE-2017-12615 <https://mp.weixin.qq.com/s?__biz=MzI1NDg4MTIxMw==&mid=2247483659&idx=1&sn=c23b3a3b3b43d70999bdbe644e79f7e5>`_
- CVE-2013-2067
- CVE-2012-4534
- CVE-2012-4431
- CVE-2012-3546
- CVE-2012-3544
- CVE-2012-2733
- CVE-2011-3375
- CVE-2011-3190
- CVE-2008-2938

Weblogic
----------------------------------------

简介
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
WebLogic是美国Oracle公司出品的一个Application Server，是一个基于Java EE架构的中间件，WebLogic是用于开发、集成、部署和管理大型分布式Web应用、网络应用和数据库应用的Java应用服务器。其将Java的动态功能和Java Enterprise标准的安全性引入大型网络应用的开发、集成、部署和管理之中。

WebLogic对业内多种标准的全面支持，包括EJB、JSP、Servlet、JMS、JDBC等。

相关CVE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
- CVE-2015-4852
    - https://github.com/roo7break/serialator
- CVE-2016-3510
- CVE-2017-3248
- CVE-2017-10271
    - http://webcache.googleusercontent.com/search?q=cache%3AsH7j8TF8uOIJ%3Awww.freebuf.com%2Fvuls%2F160367.html
- CVE-2018-2628
    - https://mp.weixin.qq.com/s/nYY4zg2m2xsqT0GXa9pMGA
- CVE-2018-2894
    - https://xz.aliyun.com/t/2458
- CVE-2018-3191
    - https://github.com/voidfyoo/CVE-2018-3191
    - https://github.com/Libraggbond/CVE-2018-3191
- CVE-2018-3197
- CVE-2018-3201
- CVE-2018-3245
- CVE-2018-3248
- CVE-2018-3252

JBoss
----------------------------------------

简介
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
JBoss是一个基于J2EE的管理EJB的容器和服务器，但JBoss核心服务不包括支持servlet/JSP的WEB容器，一般与Tomcat或Jetty绑定使用。

相关CVE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
- CVE-2017-12149

