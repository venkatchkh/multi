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
}
