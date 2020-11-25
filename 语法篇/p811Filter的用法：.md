Filter的用法：

#基础入门

1.定义一个类，实现接口，选择javax.servlet这个包，自动生成类实现的方法，在doFilter里面写入

System.out.println("filterDemo1被执行了....");

//放行，这行代码很重要，不放行不显示的

filterChain.doFilter(servletRequest,servletResponse);

2.在类方法前配置@WebFilter("/*")  //代表所有资源都会执行改过滤器

