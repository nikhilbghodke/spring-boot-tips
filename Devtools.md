# Dev Tools
ever tired of running the spring server again and again after making small changes to the application, then Dev tools is for you.

## How to use Dev Tools

Add this to ur pom.xml

```
    <dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-devtools</artifactId>
        <optional>true</optional>
    </dependency>
```

## What is Dev Tools Exactly??

Spring Boot includes an additional set of tools that can make the application development experience a little more pleasant.
The spring-boot-devtools module can be included in any project to provide additional development-time features.
To include devtools support, simply add the module dependency to your build:

### Automatic restart

Applications that use spring-boot-devtools will automatically restart whenever files on the classpath change.
This can be a useful feature when working in an IDE as it gives a very fast feedback loop for code changes.
By default, any entry on the classpath that points to a folder will be monitored for changes. 


### My automatic restart enable by dev tools will slow down your PC a bit as the server is getting restarted every now and then so use 
it carefully.

### for more info visit [docs.spring.io](https://docs.spring.io/spring-boot/docs/1.5.16.RELEASE/reference/html/using-boot-devtools.html)
