# Solution

## Complete the endpoint in the server to return the traslation

```java
TranslationResponse().apply {
    translation = "Traduceme!"    
}
```

## Build and run the server

   ```sh
   $ ./gradlew :server:build
   $ ./gradlew :server:bootRun
   ```

## Build and run the client

   ```sh
   $ ./gradlew :client:build
   $ ./gradlew :client:bootRun
   ```

## Configure GitHub actions to build work branch adding the following to the `ci.yml`

```yml
    on:
    push:
        branches: [main, work]
    pull_request:
        branches: [main, work]
```