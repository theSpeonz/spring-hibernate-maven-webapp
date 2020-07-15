node{
stage('SCM checkout')
{ 
git'https://github.com/hema1795/spring-hibernate-maven-webapp'
}
stage('clean')
{
  def mvnHome = tool name: 'maven', type: 'maven'
  bat " ${mvnHome}/bin/mvn clean "
}
}
