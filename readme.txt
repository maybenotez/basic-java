git is a good  version control system

spring 学习 


Resource  资源访问策略的抽象

todo  关于  Class.getResource  与 ClassLoader.getResource  在路径上的不同选择

ResourceLoader   资源统一加载
DefaultResourceLoader   默认实现

ProtocolResolver   通过实现此接口 来进行扩展、

ResourcePatternResolver    ResourceLoader 的扩展，它支持根据指定的资源路径匹配模式每次返回多个 Resource 实例

PathMatchingResourcePatternResolver 

what is the difference  between classpath / classpath*   https://www.cnblogs.com/EasonJim/p/6709314.html

BeanFactoryPostProcessor    通过order 来定义执行顺序
spring允许bean在实例化之前修改元数据  将bean 的 singleton修改为prototype

Spring 加载任何实现了该接口的 bean 的配置时，都会在 bean 工厂载入所有 bean 的配置之后执行 postProcessBeanFactory 方法。在 PropertyResourceConfigurer 类中实现了 postProcessBeanFactory 方法，该方法中先后调用了  mergeProperties、convertProperties、processProperties 这三个方法 ，先得到配置，将得到的配置转换为合适的类型，最后将配置内容告知 BeanFactory


BeanPostProcessor 
