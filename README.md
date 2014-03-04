This is a template-project, which uses Spring 4, Spring Security 3 and has a REST-interface for serving json-data.


<span style="color:red;font-weight:bold;">  IT IS NOT WORKING UP TO NOW  </span>


The template uses [Gradle](http://gradle.org) for dependency management and is based on the following libs:

* jackson
* hibernate
* h2
* jsonpath

It also provides the tomcat-plugin (with an embedded tomcat)

In [build.gradle](build.gradle) there is a special section with all the used versions; look at the beginning of the dependencies-section.

### HINT:
You don't need a gradle-installation because the template is using the [gradle-wrapper](http://www.gradle.org/docs/current/userguide/userguide_single.html#gradle_wrapper). But be aware that you have to use **./gradlew** or **gradlew.bat** and not *./gradle* or *gradle.bat*. 


Starting a new project
--------------------------
To get a new project up and running, just download the zip, extract it to your local workstation and navigate to the new directory.

Before starting anything you have to prepare a special directory: ```mkdir -p build/classes/main```. This is necessary for the tomcat-plugin.

Now run ```./gradlew tasks``` and sit down for a while. Gradle is fetching the dependencies and after a while you get a list with available tasks.

To test that everything is working, type ```./gradlew tomcatRun```.

After a few seconds/minutes you see ```Started Tomcat Server``` and on the next line ```The Server is running at http://localhost:8080/spring4template-rest```.

Next start yout browser and navigate to ```http://localhost:8080/spring4template-rest```. You should see the index.html file.

The template seems to be working, so it's your turn now: Happy Coding!
