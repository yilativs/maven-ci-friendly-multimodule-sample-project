This project demonstrates how to do a  multi-module CI friendly release management with Maven 3.2.1 and above.
 
It can be used without flattening plugin if it's modules are not used in other project dependencies.

Usage: 

~~~~
mvn clean install scm:tag -Drevision=$BUILD_NUMBER
~~~~

or in case you want branch to be created together with tag

~~~~
mvn clean install scm:tag scm:branch -Drevision=$BUILD_NUMBER
~~~~


Inspired by [Maven Release Plugin: Dead and Buried](https://axelfontaine.com/blog/dead-burried.html)
and
[Defining a central version in multi-module projects](https://www.mojohaus.org/flatten-maven-plugin/examples/example-central-version.html)

