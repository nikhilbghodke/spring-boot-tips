## To Add actuators to your applications


Add this to ur pox.xml
```
<dependency>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-actuator</artifactId>
</dependency>
```

In essence, Actuator brings production-ready features to our application.

Monitoring our app, gathering metrics, understanding traffic or the state of our database becomes trivial with this dependency.

The main benefit of this library is that we can get production grade tools without having to actually implement these features ourselves.

Actuator is mainly used to expose operational information about the running application – health, metrics, info, dump, env, etc. It uses HTTP endpoints or JMX beans to enable us to interact with it.

Once this dependency is on the classpath several endpoints are available for us out of the box. As with most Spring modules, we can easily configure or extend it in many ways.
