Java 8 Eclipse Patches
======================

Build an update site containing Feature Patches that can be applied to
Eclipse 4.3.

The patches are based on code in BETA_JAVA8 branches of various git
repositories on git.eclipse.org.

## Running the build

You will need a JDK8 to run the build. (Required to build org.eclipse.jdt.annotation plugin
in the jdt.core feature patch).

 1. clone this repo
 2. cd into the `git` subdirectory and run the script `java8-clone`
    This clones all the required external git repo's and checks out
    the BETA_JAVA8 branches.
 3. from the root of this repo run the commands
    "export JAVA_HOME=<path-to-a-JDK8>"
    "mvn clean install" (Requires maven 3.0 to use tycho).
    
 Upon succesfull completion an update site is built in 
   `org.springsource.ide.eclipse.java8.site/target/site`
   
 The contents of this site can be installed into an Eclipse 4.3 instance.
