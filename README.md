Thorntail Demo
===

## Prerequirements

make sure you have added the following repository to your settings.xml:  https://oss.sonatype.org/content/repositories/snapshots


## Hot Reload Example Commands

Execute commands on Terminal A

```bash:TerminalA
# Initial build
mvn package

# Run Thorntail with Development Mode
THORNTAIL_DEV_MODE=reload
./target/thorntail-demo-1.0-SNAPSHOT-bin/bin/run.sh
```

Execute commands on Terminal B

```bash:TerminalB
# Invoke Fizzed Watcher Plugin
mvn fizzed-watcher:run
```

Invoke hot reload when change a file in src directory.

You will confirm on terminal B console.

# Reference Information
* [Thorntail](https://thorntail.io/) (née WildFly Swarm)
* [Fizzed Watcher Maven Plugin](https://github.com/fizzed/maven-plugins)
