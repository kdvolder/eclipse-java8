Java 8 Eclipse Patches
======================

Build an update site containing Feature Patches that can be applied to
Eclipse 4.3.

The patches are based on code in BETA_JAVA8 branches of various git
repositories on git.eclipse.org.

## Running the build

 1. clone this repo
 2. cd into the `git` subdirectory and run the script `java8-clone`
    This clones all the required external git repo's and checks out
    the BETA_JAVA8 branches.
 3. from the root of this repo run the command
    "mvn clean install" (Requires maven 3.0 to use tycho).
    
 Upon succesfull completion an update site is built in 
   `org.springsource.ide.eclipse.java8.site/target/site`
   
 This contents of this site can be installed into an Eclipse 4.3 instance.
