# Steps to create OAR file

- Follow the ONOS directions to install the proper Maven/Karaf into your home's /Applications directory

- Then

```bash
cd apps
~/Applications/apache-maven-3.3.9/bin/mvn clean
~/Applications/apache-maven-3.3.9/bin/mvn install -DskipTests -Dcheckstyle.skip -U -T 1C

# And use the following to verify an OAR file was created

find . -name *.oar -exec ls -ls {} \;
```