hadoop-job-basic
================

This is a Maven archetype for creating a self-contained Hadoop 1.x job which
includes all its dependencies.

Before using the archetype, you have to install it in your local Maven
cache:

    $ cd hadoop-job-basic
    $ mvn clean install

Then run the archetype plugin from a different directory. You can pass a
filter argument so you don't have to pick the archetype from a huge list:

    $ mvn archetype:generate -Dfilter=de.mafr.maven.archetypes:hadoop-job-basic

Select the archetype, answer the questions and you'll find a new directory
containing your Hadoop job which you can build and run as usual:

    $ mvn clean package
    $ hadoop jar target/my-job-1.0-SNAPSHOT-job.jar


References
----------

  * [Blog article](http://blog.mafr.de/2010/07/24/maven-hadoop-job/) that
    explains the packaging setup

