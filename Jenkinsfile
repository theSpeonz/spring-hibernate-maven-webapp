pipeline {
        agent any tools{
                tool name: 'maven3', type: 'maven'
        }
        stages{
stage('SCM checkout')
{ 
git'https://github.com/hema1795/spring-hibernate-maven-webapp'
}
        stage('Build') {
         
        }
        stage('test') {
               bat 'mvn test'
        }
        stage('Deploy') {
          bat 'mvn deploy'
        }
  
stage('clean')
{
  bat 'mvn clean '
}
}
}
