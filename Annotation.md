# 1. Using the @SpringBootAppliaction Annotation
   This annotation can be used to enale those three featrues, that is:
   * @EnableAutoConfiguration：enable Spring Boot‘s auto-configuration mechanism.
   * @ComponentScan: enable Component scan on the package.
   * @Configuration allow to register extra beans in the context or import additional confguration calsses.
  that means @SpringBootApplication // same as @Configuration @EnableAutoConfiguration @ComponentScan
## 1.1 @ComponentScan
    Either basePackageClasses() or basePackages() (or its alias value()) may be specified to define specific
    packages to scan. If specific packages are not defined, scanning will occur from the package of the class
    that declares this annotation.
## 1.2 @EnableAutoConfiguration
    Auto-configuration tries to be as intelligent as possible and will back-away as you define more of your own
    configuration. You can always manually exclude() any configuration that you never want to apply (use excludeName()
    if you don't have access to them). You can also exclude them via the spring.autoconfigure.exclude property. 
    Auto-configuration is always applied after user-defined beans have been registered.
    
  
