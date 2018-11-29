# Build Instructions

## Create new Splunk Application Bundle

* Update version number in `gradle.properties`

```version=1.0.0```

* Run gradle:

```./gradle createDist

distName: TA-vectra-cognito-1.0.0.spl
destinationDir: <repositorypath>/TA-vectra-cognito/build/distributions
:createDist

BUILD SUCCESSFUL

Total time: 0.993 secs
```

* A new `TA-vectra-coginit-<version>.spl` package will be created in the build/distributions directory

## Prepare app certification

to be done