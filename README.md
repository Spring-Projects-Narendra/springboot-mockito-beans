# springboot-mockito-beans

https://spring.io/blog/2016/04/15/testing-improvements-in-spring-boot-1-4

Some important things from above url:

From springboot 1.4 there are changes in spring-test

@RunWith(SpringJUnit4ClassRunner.class) - > @RunWith(SpringRunner.class) [simplified name]

@SpringApplicationConfiguration(MyApp.class) - > @SpringBootTest

Attributes of  SpringBootTest:

<b>classes</b> : If we want to load a specific configuration, we can use the classes attribute of @SpringBootTest. In this example, we’ve omitted classes which means that the test will first attempt to load @Configuration from any inner-classes, and if that fails, it will search for your primary @SpringBootApplication class.

