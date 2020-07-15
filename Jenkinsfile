node{
stage('SCM checkout')
{ 
git 'https://github.com/theSpeonz/spring-hibernate-maven-webapp'
}
stage('clean')
{
  def mvnHome = tool name: 'maven3', type: 'maven'
  bat " ${mvnHome}/bin/mvn clean "
}
}
