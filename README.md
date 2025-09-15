## Creating a Project
docker run --rm -it -v ./:/app -w /app maven:latest mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=. -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

-DartifactId=. (current directory)

## Build the Project
docker run --rm -it -v ./:/app -w /app maven:latest mvn package

test