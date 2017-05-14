# Wiremock example with Body Transformer

### Start server

```
java -cp "wiremock-body-transformer-1.1.5.jar:wiremock-2.6.0-standalone.jar" com.github.tomakehurst.wiremock.standalone.WireMockServerRunner --verbose --extensions com.opentable.extension.BodyTransformer
```

### Reload mappings

When new stub is added while the mock server is running:

```
POST localhost:8080/__admin/mappings/reset
```

### Use of priority

`priority` is used when there is overlap between stubs and the stub with more specific conditions should have higher priority (smaller value).

### See more

- [Wiremock docs](https://wiremock.org/docs/getting-started/)
- [Wiremock Body Transformer](https://github.com/opentable/wiremock-body-transformer)
