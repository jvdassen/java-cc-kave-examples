# java-cc-kave-examples

## Fetch dependencies and build JAR file
```bash
mvn package
```
## Run the examples

Supply the project directory and where the KaVE datasets can be found. Note the ```/``` at the end of `BASE_DIR`.

The examples should be run with at least 8gb of memory.

```bash
export BASE_DIR=/home/user/path/to/project/
export EVENTS_SUBDIR=datasets/Events_123456/
export CONTEXTS_SUBDIR=datasets/Contexts_123456/
export JVM_MEMORY=10G

# Optionally variable to skip the mining step
export SKIP_MINING=TRUE

java -Xmx${JVM_MEMORY} -cp target/examples-0.0.1-SNAPSHOT.jar RunMe 
```
