node{
stage('SCM checkout')
{ 
git'https://github.com/hema1795/spring-hibernate-maven-webapp'
}
        stage('Build') {
         
        }
        stage('Test') {steps {
                sh 'mvn test'
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
                
           
        }
        stage('Deploy') {
          
        }
  
stage('clean')
{
  def mvnHome = tool name: 'maven3', type: 'maven'
  bat " ${mvnHome}/bin/mvn clean "
}
}
