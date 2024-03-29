pipeline {
    agent any
    
    tools {
        gradle 'Gradle87'
    }

    stages {
        stage('Clone') {
            steps {
                git branch: 'master', url: 'https://github.com/Nengsopheap/Midterm-devop.git'
            }
        }
        stage('Build'){
            steps{
                sh 'gradle clean build'
            }
        }
    }
}