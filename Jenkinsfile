node{
stage('SCM checkout')
{ 
git'https://github.com/hema1795/spring-hibernate-maven-webapp'
}
        stage('Build') {
         
        }
        stage('Test') {
           bat 'mvn Test'
        }
        stage('Deploy') {
          bat 'mvn Deploy'
        }
  
stage('clean')
{
  def mvnHome = tool name: 'maven3', type: 'maven'
  bat " ${mvnHome}/bin/mvn clean "
}
}
