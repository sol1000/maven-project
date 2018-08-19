# maven-project
Source code for James Lee's Jenkins course.

Check out our Latest DevOps PDF book.

https://www.level-up.one/devops-pdf-book

# install maven and tomcat
/Users/slim/tools/apache-maven-3.5.4/
/Users/slim/tools/apache-tomcat-8.5.32-prod/
/Users/slim/tools/apache-tomcat-8.5.32-staging/

# fully automated jenkins pipeline
tomcat_dev
ssh -i tomcat-demo.pem ec2-user@52.55.10.130
tomcat_prod
ssh -i tomcat-demo.pem ec2-user@18.207.0.114

- as ec2-user
sudo yum install tomcat7
cd /etc/tomcat7/
ls -ltr
cd /var/lib/tomcat7
ls -al
cd webapps/
ls -al
sudo service tomcat7 start

- with a root permission
cd /var/log/tomcat7


http://52.55.10.130:8080/webapp
http://18.207.0.114:8080/webapp

scp -i /Users/slim/.ssh/tomcat-demo.pem /var/lib/tomcat8/webapps/webapp.war ec2-user@52.55.10.130:/var/lib/tomcat7/webapps
