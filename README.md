#USERS
```
# apt update
# apt-get install openjdk-8-jdk
# java -version
# apt install mavn

    Now, go and fetch git code

# git clone https://github.com/zelar-soft-todoapp/users.git
# cd users
# mvn clean package
# java -jar target/users-api-0.0.1.jar

    Start service now

# vi /etc/systemd/system/users.service
# systemctl daemon-reload
# systemctl start users
# systemctl enable users

```