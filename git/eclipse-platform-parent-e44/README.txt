The files in here are almost verbatim copied from the 
'eclipse.platform.releng.aggregrator'.

In particular this contents of the 'eclipse-platform-parent' folder
was copied to the expected relative position w.r.t. to eclipse.jdt.core (and 
other git clones) as references from their pom files.

The eclipse-platform-parent/pom.xml was then modified in the following way:
  - added Eclipse 4.3 update site:  to be able to resolve E43 dependencies
    without having to checkout and build all of the eclipse 4.3 source code.
