# jfs

JFS provides a copy of Jetty with Fedora and Solr preinstalled and ready to run.

* [Fedora repository](https://github.com/futures/fcrepo4)
* [Solr](http://lucene.apache.org/solr/)

Adapted from [hydra-jetty 7.x-stable](https://github.com/projecthydra/hydra-jetty/tree/7.x-stable)

## Included Versions

* jetty: 8.1.16
* solr: 4.10.2
* fedora: 3.8.1

## Usage

### Dependencies

* [Java 8 (JRE)](https://java.com/en/download/index.jsp)


### Manual

    git clone https://github.com/emory-lits-labs/jfs
    cd jfs
    ./start.sh

### Interaction

When jetty is finished initializing itself, Solr has development and test cores and is available at:

* [http://localhost:8080/solr/](http://localhost:8080/solr/)

Fedora is available in two copies, one for developement:

* [http://localhost:8080/fedora/](http://localhost:8080/fedora/)

and an additional copy for testing:

* [http://localhost:8080/fedora-test/](http://localhost:8080/fedora-test/)

You can see a list of all installed applications at

* [http://localhost:8080](http://localhost:8080)

### Updating

#### Solr and Jetty

Solr is updated by downloading the latest from [Lucene](http://lucene.apache.org/solr/), which includes an instance of Jetty in the
`example` directory.  Updating is a process of replacing the jar files as well as the solr.war and start.jar files.  Note that the
example from Lucene does not include the start.ini file.

