# Springboot 集成 JSP

## Idea Project 集成 JSP 和 Idea Module 集成 JSP 的不同

### Idea Project 集成 JSP 输出
```log
2021-06-08 17:40:56.111 DEBUG 14932 --- [nio-8081-exec-3] org.apache.jasper.servlet.JspServlet     : JspEngine --> /WEB-INF/pages/hello.jsp
2021-06-08 17:40:56.111 DEBUG 14932 --- [nio-8081-exec-3] org.apache.jasper.servlet.JspServlet     : 	     ServletPath: /WEB-INF/pages/hello.jsp
2021-06-08 17:40:56.111 DEBUG 14932 --- [nio-8081-exec-3] org.apache.jasper.servlet.JspServlet     : 	        PathInfo: null
2021-06-08 17:40:56.115 DEBUG 14932 --- [nio-8081-exec-3] org.apache.jasper.servlet.JspServlet     : 	        RealPath: E:\GITHUB\springboot-jsp-example\src\main\webapp\WEB-INF\pages\hello.jsp
2021-06-08 17:40:56.115 DEBUG 14932 --- [nio-8081-exec-3] org.apache.jasper.servlet.JspServlet     : 	      RequestURI: /WEB-INF/pages/hello.jsp
2021-06-08 17:40:56.115 DEBUG 14932 --- [nio-8081-exec-3] org.apache.jasper.servlet.JspServlet     : 	     QueryString: null
```

### Idea Module 集成 JSP 输出
```log
2021-06-08 17:40:40.155 DEBUG 6024 --- [nio-8080-exec-4] org.apache.jasper.servlet.JspServlet     : JspEngine --> /WEB-INF/pages/hello.jsp
2021-06-08 17:40:40.155 DEBUG 6024 --- [nio-8080-exec-4] org.apache.jasper.servlet.JspServlet     : 	     ServletPath: /WEB-INF/pages/hello.jsp
2021-06-08 17:40:40.156 DEBUG 6024 --- [nio-8080-exec-4] org.apache.jasper.servlet.JspServlet     : 	        PathInfo: null
2021-06-08 17:40:40.162 DEBUG 6024 --- [nio-8080-exec-4] org.apache.jasper.servlet.JspServlet     : 	        RealPath: C:\Users\27812\AppData\Local\Temp\tomcat-docbase.8080.17694328029717503144\WEB-INF\pages\hello.jsp
2021-06-08 17:40:40.162 DEBUG 6024 --- [nio-8080-exec-4] org.apache.jasper.servlet.JspServlet     : 	      RequestURI: /WEB-INF/pages/hello.jsp
2021-06-08 17:40:40.162 DEBUG 6024 --- [nio-8080-exec-4] org.apache.jasper.servlet.JspServlet     : 	     QueryString: null
```

两种不同形式的 RealPath 不同

目前没搞懂区别，并且 Module 的形式会出现找不到 jsp 文件
