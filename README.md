#log


###2016/3/13
####很久就想搞一个类似于个人网站的玩意，放在tomcat里跑跑,也可以以项目来驱动自己学习。
####初步完成 spring,springMVC环境的搭建，暂时不用ORM框架，以后可以玩玩MyBatis.


###2016/3/14
####spring MVC 静态资源的问题 最好放在webapp目录下
####页面使用Free Bootstrap Theme--Worthy


###2016/3/15
####前端施工中，主页：修改CSS, 添加背景图片


###2016/3/16
####单例模式 静态工厂方法 DateUtil
#### 搞清楚spring mvc的viewResolver到底怎么用 搞了一下午一晚上还是不怎么清楚啊日
#### ViewandModel......

###2016/3/20
####working.....hate css.

###2016/3/21
####算了，还是搞个简单的图书管理系统吧


###2016/3/22
####注册功能施工中....
####客户端密码校验 

###2016/3/23
####持久层框架用 MyBatis试试
####正在整合Spring和MyBatis....好多配置文件啊啊啊啊

###2016/3/24
####配置文件好多...有点混乱...先把MyBatis整清楚再去整合Spring吧


###2016/3/24
####用注解+接口的方式还是直接用xml?  它们之间的关系？ 其实是用接口去对应xml文件？ 接口是用来绑定的？
####“当你程序需要执行的时候，系统会去寻找对应的sql语句，
你如果存在两个 那么系统就会迷茫 不知道该选择哪一个 所以就报错了  
xml格式最后在编译的时候也是存放在内存中，相当于一段代码
所以他和注解表示的作用是一样的 两个一样的东西 最后系统选择的时候肯定会报错的 因为不知道选哪一个”####
####原来两种方式其实是一样的


###2016/3/26
####xml文件中的 namespace是用来绑定接口的 官方文档还是建议用映射文件，功能更强大，注解的方式更适合执行一些简单的sql语句
####<select>标签中的id属性对应的是接口中方法的名称
####再用注解来试试
####啊啊啊啊 为什么 <bean id="sqlSessionFactory" class="org.mybatis.spring.SqlSessionFactoryBean">
		<property name="dataSource" ref="dataSource" />
		<property name="configLocation" value="classpath:MyBatis-Configuration.xml"></property>
	</bean> 这个不加 就接口就和xml绑定不了啊啊啊阿   fxxxxxxxxxxx 弄了一下午####