pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bsbbuggywebapp -Dsonar.organization=bsbbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=ac80374ee998f5ae708fdb5aafe440e4098d308b'
			}
        } 
  }
}
