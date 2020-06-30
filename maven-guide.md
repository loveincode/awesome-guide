```
1. 创建Maven的普通Java项目：
mvn archetype:create
    -DgroupId=packageName
    -DartifactId=projectName

2. 创建Maven的Web项目：
mvn archetype:create
    -DgroupId=packageName
    -DartifactId=webappName
    -DarchetypeArtifactId=maven-archetype-webapp

mvn compile          编译源代码
mvn test-compile     编译测试代码
mvn test             运行测试
mvn package          打包，根据pom.xml打成war或jar
    如果pom.xml中设置 war，则此命令相当于mvn war:war
    如果pom.xml中设置 jar，则此命令相当于mvn jar:jar

mvn -Dtest package   打包但不测试。完整命令为：mvn -D maven.test.skip=true package
mvn install          在本地Repository中安装jar
mvn deploy           上传到私服
mvn clean            清除产生的项目

mvn dependency:sources 下载源码

mvn jar:jar         只打jar包

mvn eclipse:clean   清除eclipse的一些系统设置
mvn eclipse:eclipse 生成eclipse项目
mvn idea:idea       生成idea项目

出现 pom.part.lock，访问也超时，nexus超时，重启能解决
```
