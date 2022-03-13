## Q&A  
### production-ready特性的含义是什么？？  
答案：待解答

### 自动装配的进化史  ？  
低版本Spring Framework时代   
xml配置

spring framework 2.5 时代
annotation逐步取代xml配置，@Component注解等等

spring framework 3.0 时代
@Configuration @Bean等等替代"\<bean>", @Import注解

spring framework 3.1 时代
@ComponentScan代替xml的scan标签,和ImportSelector接口

spring framework 4.0 时代
@Conditional的引入，让选择性装配成为可能