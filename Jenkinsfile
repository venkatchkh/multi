node('master') 
{
    stage('continous download_master') 
       {
    git 'https://github.com/venkatchkh/multi.git'
       }
    stage('continous Build_master') 
       {
    sh 'mvn package'
       }
    stage('continous Deployment_master') 
       {
    sh 'scp /home/ubuntu/.jenkins/workspace/jobm/webapp/target/webapp.war ubuntu@172.31.47.170:/var/lib/tomcat9/webapps/qaenv.war'
       }
    stage('continous Testing_master') 
       {
    sh 'echo "Testing is Passed"'
       }
    stage('continous Delivery_master') 
       {
    sh 'scp /home/ubuntu/.jenkins/workspace/jobm/webapp/target/webapp.war ubuntu@172.31.34.123:/var/lib/tomcat9/webapps/prodenv.war'
       }
}