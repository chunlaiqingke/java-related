### 第三章 理解固化的maven依赖

#### Maven的Scope
https://www.jianshu.com/p/a4fc54b5a6bf  
compile  
表示 dependency 可以在生命周期中使用。而且这些dependencies 会传递到依赖的项目中。  

provided  
跟compile相似，但是表明了dependency 由JDK或者容器提供。
例如Servlet AP和一些Java EE APIs。这个scope 只能作用在编译和测试时，同时没有传递性。
使用这个时，不会将包打入本项目中，只是依赖过来。


runtime  
表示dependency不作用在编译时，但会作用在运行和测试时  

test  
表示dependency作用在测试时，不作用在运行时。

system  
跟provided 相似，但是在系统中要以外部JAR包的形式提供，maven不会在repository查找它

import  
它只使用在dependencyManagement中，表示从其它的pom中导入dependency的配置
