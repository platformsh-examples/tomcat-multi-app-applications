# Tomcat multi-app template for Platform.sh

The Apache Tomcat® software is an open source implementation of the Java Servlet, JavaServer Pages, Java Expression Language and Java WebSocket technologies. The Java Servlet, JavaServer Pages, Java Expression Language and Java WebSocket specifications are developed under the Java Community Process.

This template has the Tomcat, so you need to deploy your application with Codehaus Cargo

## Services

* Java 8

## Customizations

The following files and additions make the framework work.  If using this project as a reference for your own existing project, replicate the changes below to your project.

* [`.platform/routes.yaml`](.platform/routes.yaml): Platform.sh allows you to define the [routes](https://docs.platform.sh/configuration/routes.html).
* [`.platform/services.yaml`](.platform/services.yaml):  Platform.sh allows you to completely define and configure the topology and [services you want to use on your project](https://docs.platform.sh/configuration/services.html).
* [`.platform/applications.yaml`](.platform/applications.yaml): It is possible to define an application in a .platform/applications.yaml file in addition to discrete .platform.app.yaml files. The syntax is nearly identical, but the source.root key is required. The applications.yaml file is then a YAML array of application definitions.
* An additional library dependency, [`platformsh/config-reader-java`](https://github.com/platformsh/config-reader-java), has been added.  It provides convenience wrappers for accessing the Platform.sh environment variables.

## References

* [Platform.sh post](https://platform.sh/blog/2019/java-hello-world-at-platform.sh/)
* [Apache Tomcat](http://tomcat.apache.org/)
* [Java at Platform.sh](https://docs.platform.sh/languages/java.html)
* [Platform.sh Multi-app](https://docs.platform.sh/configuration/app/multi-app.html)
