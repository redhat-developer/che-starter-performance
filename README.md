# Performance tests for che-starter
Che starter performance tests performance of che-starter server by calling its API with numerous amount of requests.

## How to run
- run `mvn clean integration-test` from command line

## Execution parameters
- `che.starter.host` - che-starter host (hostname:port), default `localhost:10000`
- `vertx.server` - Vertx server, which is used as OpenShift server (masterURL), default `http://localhost:33333`

## Performance results
Results are located in target folder and its subfolders. There is output from console in perfcake-maven-plugin.log as well as charts for performance.