How To
=====================

1. Clone project
```
https://github.com/timveil/ambari-view-archetype.git
```
2. Install `ambari-view-archetype` in your local Maven Repository
```
mvn install
```
3. Execute the following to generate your new Ambari View project from the `ambari-view-archetype`
```
mvn archetype:generate \
-DgroupId=[CHANGE_ME] \
-DartifactId=[CHANGE_ME] \
-Dversion=[CHANGE_ME] \
-Dpackage=[CHANGE_ME] \
-DviewName=[CHANGE_ME] \
-DviewLabel=[CHANGE_ME] \
-DarchetypeGroupId=ambari-view-archetype \
-DarchetypeArtifactId=ambari-view-archetype \
-DarchetypeVersion=1.0-SNAPSHOT \
-DarchetypeCatalog=local \
-DinteractiveMode=false

```
4.  Once you've created your new view project, you can run `mvn package` to create the `*-view.jar`.  The new view can be deployed on your Ambari server by dropping it in `/var/lib/ambari-server/resources/views`
