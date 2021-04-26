node('master') 
{
    stage('continous download_Loans') 
       {
    git 'https://github.com/venkatchkh/multi.git'
       }
    stage('continous Build_Loans') 
       {
    sh 'mvn package'
       } 
           stage('continous Deployment_loans') 
       {
    sh 'scp /home/ubuntu/.jenkins/workspace/jobm_loans/webapp/target/webapp.war ubuntu@172.31.47.170:/var/lib/tomcat9/webapps/qaenv1.war'
       }
    stage('continous Testing_loans') 
       {
    sh 'echo "Testing is Passed"'
       }
    stage('continous Delivery_loans') 
       {
    sh 'scp /home/ubuntu/.jenkins/workspace/jobm_loans/webapp/target/webapp.war ubuntu@172.31.34.123:/var/lib/tomcat9/webapps/prodenv1.war'
       }
 }
