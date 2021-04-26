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
}