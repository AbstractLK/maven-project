## Creating a Project (.war)
<!-- docker run --rm -it -v ./:/app -w /app maven:latest mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=. -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false -->
#### Instead of quickstart, use the maven-archetype-webapp
docker run --rm -it -v ./:/app -w /app maven:latest mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=mywebapp -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false


### -DartifactId=mywebapp (project directory)

## Build the Project
docker run --rm -it -v ./:/app -w /app maven:latest mvn package

