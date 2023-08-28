# Opendata services

## Build & run

### Requirements

Those components are created with the following requirements:
* Java 17 JDK
* Maven 3.8+
* Docker


### Building

Compile, test, install:

```shell script
./mvnw clean install
```

Build docker image:

```shell script
./mvnw clean package -Pdocker
```

### Running

See the [OGC Features API](src/services/ogc-features/README.md) documentation for more information.

### Development/debug

To run one service directly without docker, use the `local` profile.

```shell script
mvn spring-boot:run -Dspring-boot.run.profiles=dev,local -f src/services/data-indexer/
```

## Bugs

TBD

## Roadmap

TBD

## Contributing

To set license header use:

```shell script
./mvnw license:format
```
