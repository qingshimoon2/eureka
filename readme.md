eureka集群配置

- 1.配置本地hosts
> 127.0.0.1 eurekaA <br>
> 127.0.0.1 eurekaB

- 2.创建两个配置文件application-a.properties和application-b.properties
- 3.打包程序
- 4.分别启动两个实例
```shell script
java -jar eureka-0.0.1-SNAPSHOT.jar --spring.profiles.active=a
```

```shell script
java -jar eureka-0.0.1-SNAPSHOT.jar --spring.profiles.active=b
```

- 5.分别访问http://localhost:1111/ 和 http://localhost:1112/

