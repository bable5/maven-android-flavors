Maven Android Build Flavors
====

This project is a working implementation of the discussion in the 
[Branded Android Builds using Maven](http://tech.ebuddy.com/2013/04/08/branded-android-builds-using-maven/)
blog post.

The project demonstrates how to create builds for two different types of builds,
dev and release. The different build environments provide unique values for the
resource 'search'.

Building and Deploying to a Connected Device
----

The <code>environment</code> property controlls which files are used for 
the build. Valid values are <code>dev</code> and <code>release</code>.

* Dev build/install

````bash
$> mvn -Denvironment=dev package android:deploy
````

* Release build/install

````bash
$> mvn -Denvironment=release package android:deploy
````

