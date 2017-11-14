This is from talk from mmacik - mail to Tom Jenkinson from 2017-11-14.

You simply run it by running module jbpm-performance-tests with this
command:

mvn clean install exec:exec -Dsuite=ConcurrentLoadSuite -Dscenario=LStartEndProcess -Dthreads=1 -Dversion.org.kie=7.3.1-SNAPSHOT


Notice -Dthreads=1 part - with one thread it should be OK, with
-Dthreads=4 or 8 or 16 it should throw exceptions I mentioned.
