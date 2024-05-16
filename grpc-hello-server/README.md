# grpc-codelab-hello

Based on https://codelabs.developers.google.com/codelabs/cloud-grpc-java

3. Create a gRPC Service

```shell
mvn archetype:generate -DgroupId=com.example.grpc \
 -DartifactId=grpc-hello-server \
 -DarchetypeArtifactId=maven-archetype-quickstart \
 -DinteractiveMode=false
 
cd grpc-hello-server

mvn -DskipTests package

touch src/main/java/com/example/grpc/GreetingServiceImpl.java

mvn -DskipTests package exec:java -Dexec.mainClass=com.example.grpc.App

touch src/main/java/com/example/grpc/Client.java

mvn -DskipTests package exec:java -Dexec.mainClass=com.example.grpc.Client

```
