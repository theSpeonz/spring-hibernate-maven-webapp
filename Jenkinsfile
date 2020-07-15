node{
stage('SCM checkout')
{ 
git 'https://github.com/theSpeonz/spring-hibernate-maven-webapp'
}
stage('clean')
{
  def mvn_version = 'M3'
  def mvnHome = tool name: 'maven3', type: 'maven'
  bat " ${mvnHome}/bin/mvn clean "
}
}
