# Auto Logging of Method Invocation in Java
Inspired from The Pragmatic Programmer (p. 40) on easily adding tracing capability to method invocation via logging.

Investigate Java annotations and adding method invocation that way, or even method invocatioin via Java reflection on the base object class.

## Investigation
Learning about Java annotations: [Oracle Java Tutorials](https://docs.oracle.com/javase/tutorial/java/annotations/basics.html) and [Custom Java Annotations Example](https://www.mkyong.com/java/java-custom-annotations-example/).

It appears that it's fairly easy to create Java annotations.  However, to access the annotations, you need to have a custom way to run the program.  You have to gather the classes with the expected annotations, process the annotations, and then execute the method.  (This clarifies how JUnit works).

During my investigation, I also learned about [AOP Logger](http://www.yegor256.com/2014/06/01/aop-aspectj-java-method-logging.html).  I would still like to explore method invocation programatically and intercepting bytecode execution on the fly (apparently using [class loaders](https://en.wikipedia.org/wiki/Java_Classloader)).
