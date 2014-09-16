# Cascading Sample Applications

This is a collection of trivial applications written in Cascading. 

Cascading is an API for building data oriented applications in Java on Apache Hadoop, Apache Tez, or other 
emerging platforms.

To keep things simple, all these samples require Apache Tez to be installed.

For illustrative purposes, a trivial application written against the Hadoop MapReduce API, is available. It does
not require Tez libraries.

## Sample Applications

Each sub-project in this project are completely stand-alone and made available for download independently in the
[Cascading SDK](http://www.cascading.org/sdk/).

* logparser - trivially parse a Apache web server log into a text delimited file, with field names
* loganalysis - extends `logparser` to provide basic analytics and break up the application into logical components
* wordcount - showcases the use of reusable sub-assemblies to process complex data sets
* hadoop - a trivial MapReduce example as contrast to the Cascading examples

All the Cascading samples use the same build file (see sample.build.gradle).

## Building and IDE Integration

For most cases, building Cascading is unnecessary as it has been pre-built, tested, and published to our Maven
repository (above).

To build Cascading, run the following in the shell:

```bash
> git clone https://github.com/Cascading/cascading.samples
> cd cascading.samples
> gradle build
```
Cascading requires Gradle 1.12 and Java 1.7 to build.

To use an IDE like IntelliJ, run the following to create IntelliJ project files:

```bash
> gradle idea
```

Similarly for Eclipse:

```bash
> gradle eclipse
```

## Getting Help

Please post any questions to the Cascading mail list, which can be reached from the Cascading site: http://cascading.org/

## Contributing

Please fee free to fork and offer up pull requests for any other sample applications that might be illustrative of
Cascading features.

Would also love to see a raw Tez sample added as well.