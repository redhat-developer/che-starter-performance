# Performance tests for che-starter
Che starter performance tests performance of che-starter server by calling its API with numerous ammount of requests.

## How to run
- run `mvn clean integration-test` from command line

## Execution parameters
- `che.starter.host` - che-starter host (hostname:port)
- `vertx.server` - Vertx server, which is used as OpenShift server (masterURL)

## Performance results
Results are located in target folder. There is output from consoel in perfcake-maven-plugin.log as well as charts for performance.