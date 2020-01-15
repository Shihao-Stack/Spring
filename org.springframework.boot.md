# 1. SpringAllication
    Class that can be used to bootstrap and launch a Spring application from a Java main method. 
    By default class will perform the following steps to bootstrap your application
    
      * Create an appropriate ApplicationContext instance (depending on your classpath)
      * Register a CommandLinePropertySource to expose command line arguments as Spring properties
      * Refresh the application context, loading all singleton beans
      * Trigger any CommandLineRunner beans
      
## 1.1 run()    
    In most circumstances the static run(Class, String[]) method can be called directly from your main 
    method to bootstrap your application:
```
      @Configuration
      @EnableAutoConfiguration
      public class MyApplication  {

        // ... Bean definitions

        public static void main(String[] args) {
          SpringApplication.run(MyApplication.class, args);
        }
      }
```
