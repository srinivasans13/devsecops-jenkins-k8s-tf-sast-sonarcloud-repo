pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggyweapp -Dsonar.organization=buggyweapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=41ecf292b104568f2959c655098795579880c245'
			}
        } 
  }
}
