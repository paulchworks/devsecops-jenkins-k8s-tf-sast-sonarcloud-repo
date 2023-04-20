pipeline {
  agent any
  tools { 
        maven 'Maven_2_3_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=paulchbuggywebapp -Dsonar.organization=paulchbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9e1adcf913928573e907404d7c262982343b8363'
			}
        } 
  }
}
