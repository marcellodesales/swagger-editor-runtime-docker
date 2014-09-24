Swagger-Editor-Runtime Docker dependencies
------

This repository contains the Dockerfile for building the runtime
dependency for the Swagger Editor.

Build
------

Just run the regular Docker commands.

```
docker build -t marcellodesales/swagger-editor-runtime .
```

Reuse
----

Just use a FROM instruction in a parent Dockerfile.

```
###
# Swagger-editor runtime dependency with all the needed dependencies installed.
# This dependency will automatically call "grunt serve" after the installation
# on this layer is performed.
###
FROM marcellodesales/swagger-editor-runtime
MAINTAINER Marcello_deSales@intuit.com
```
