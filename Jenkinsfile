pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappcourse -Dsonar.organization=asgbuggywebappcourse -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=11041946e4491fc5b169e015ca48adb9d0657979'
			}
        } 
  }
}
