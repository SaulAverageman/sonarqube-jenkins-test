pipeline{
    agent any
    tools{
        maven 'MAVEN'
    }

    stages{
        stage('run sonarqube'){
            steps{
                script{
                    withSonarQubeEnv('sonar-server'){
                        sh 'mvn sonar:sonar'
                    }
                }
            }
        }
    }
    
}