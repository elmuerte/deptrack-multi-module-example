Example project to test multi module handling of the [maven dependency-track plugin](https://github.com/pmckeown/dependency-track-maven-plugin).

Run with:

```
mvn -fae -pl child1,child2 -Ddependency-track.dependencyTrackBaseUrl=http://localhost:8080 -Ddependency-track.apiKey=xxyyzz cyclonedx:makeBom dependency-track:upload-bom dependency-track:findings
```

Both modules have a critical finding, but different versions for the affected dependency.
