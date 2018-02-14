# fuse-edit-log-level-on-certain-container
This is tutorial how to change log level on certain container

1. go to your jboss fuse parent container

2. go to /bin folder

3. run ./client

4. #> container-connect <container that you want to edit select just 1>

5. #> config:edit org:ops4j.pax.logging

6. #> config:propset log4j.rootLogger "DEBUG, out, osgi:VmLogAppender" <-- depends on which level you want

7. #> config:update

8. check your hawtio and go to the container that you have changed, it will change to the level you want.
