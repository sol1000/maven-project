# maven-project
Source code for James Lee's Jenkins course.

Check out our Latest DevOps PDF book.

https://www.level-up.one/devops-pdf-book

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


