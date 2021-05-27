#USERS
```
Users service is responsible for finding the users by username and password.

    First you need to downgrade java version from java-11 to java-8

# apt update
# apt-get remove openjdk-11-jdk-headless
# apt-get install openjdk-8-jdk
# java -version
# apt install maven

    Now, go and fetch git code

# git clone https://github.com/zelar-soft-todoapp/users.git
# cd users
# mvn clean package
# java -jar target/users-api-0.0.1.jar

    Start service now

# mv /root/users/systemd.service /etc/systemd/system/users.service
# systemctl daemon-reload
# systemctl start users
# systemctl enable users
```
#RELEASE TAG 0.0.1