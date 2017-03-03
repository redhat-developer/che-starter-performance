# Performance tests for che-starter
Che starter performance tests performance of che-starter server by calling its API with numerous amount of requests.

## How to run
- run `mvn clean integration-test` from command line

## Execution parameters
- `che.starter.host` - che-starter host (hostname:port), use `localhost:10000` when running locally with mocked vertx che server 
- `vertx.server` - Vertx server, which is used as OpenShift server (masterURL), use `http://localhost:33333` when running locally with mocked vertx che server
-`perfcake.scenario` - perfcake scenario to run

## PerfCake scenarios
All scenarios try to create a workspace on OpenShift. Different is only in rate of messages and count of messages.
- `create-workspace-scenario` - message rate 150/s, message count 3000, estimated duration 20 seconds
- `soak` - message rate 50/s, message count 30000, estimated duration 10 minutes
- `storm` - message rate 500/s, message count 5000, estimated duration 10 seconds

## Performance results
Results are located in target folder and its subfolders. There is output from console in perfcake-maven-plugin.log as well as charts for performance.
