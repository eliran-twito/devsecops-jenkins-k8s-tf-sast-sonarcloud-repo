pipeline {
  agent any
  tools { 
        maven 'maven_3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=DevSecOps_test11 -Dsonar.organization=DevSecOps_test11 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=9376e2a20cbb2139a79d90926fcfda3aa0d817e3'
			}
        } 
  }
}
