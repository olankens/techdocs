<hr>

<div align="center">
  <p><img src="../.assets/spring.svg" width="128"/></p>
  <h1>SPRING</h1>
</div>

### Update Gradle Wrapper

```shell
version="$(curl -s https://services.gradle.org/versions/current | jq -r .version)"
./gradlew wrapper --gradle-version "$version"
```

<hr>

### Update Maven Wrapper

```shell
address="https://maven.apache.org/download.cgi"
pattern="Apache Maven [0-9]+\.[0-9]+\.[0-9]+"
version="$(curl -s "$address" | grep -A2 'id="CurrentMaven"' | grep -oE "$pattern" | head -1 | awk '{print $3}')"
./mvnw -N wrapper:wrapper -Dmaven="$version"
```

<hr>
