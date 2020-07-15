node{
stage('SCM checkout')
{ 
git 'https://github.com/theSpeonz/spring-hibernate-maven-webapp'
}
stage('clean')
{
  def mvnHome = tool name: 'maven', type: 'maven'
  bat " ${mvnHome}/bin/mvn clean "
}
}
