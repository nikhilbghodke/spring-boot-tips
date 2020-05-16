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


## For easy interface to navigate your API use HAL Browser

add this to your pom.xml to start HAL browser

```
                <dependency>
		    <groupId>org.springframework.data</groupId>
		    <artifactId>spring-data-rest-hal-browser</artifactId>
		</dependency>
```
## Exposing Endpoints in actuators

Actuator endpoints let you monitor and interact with your application. Spring Boot includes a number of built-in endpoints and lets you add your own. For example, the health endpoint provides basic application health information.

Each individual endpoint can be enabled or disabled and exposed (made remotely accessible) over HTTP or JMX. An endpoint is considered to be available when it is both enabled and exposed. The built-in endpoints will only be auto-configured when they are available. Most applications choose exposure via HTTP, where the ID of the endpoint along with a prefix of /actuator is mapped to a URL. For example, by default, the health endpoint is mapped to /actuator/health.

By default only few endpoibnts are enabled in web form , that might be cause of security concerns.

### To enable all actuators enpoints

Add this to application.properties file

```
management.endpoints.web.exposure.include=*
```

Ebndpoints aregive you every interesting information, please refer to this documentaion for more info on actuator endpoints [docs.spring.io](https://docs.spring.io/spring-boot/docs/current/reference/html/production-ready-features.html).

#### Disclaimer by enabling monitoring by actuator it will degrade the performance of your application and thus should be used in production.
