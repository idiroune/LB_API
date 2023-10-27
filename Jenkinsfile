pipeline {
    agent any
    tools {
        maven 'MavenJenkins2'
    }
    stages {
        stage('Clone Git repository'){
            steps{
                git url: 'https://balgitlab01.eutelsat.fr/eutelsat/LB-API.git'
            }
        }
        stage('Compile') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
