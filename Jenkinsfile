pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: '*/main', url: 'https://github.com/Crush-Steelpunch/BAE14-repo.git'
            }
        }
        stage('Run') {
            steps {
                sh 'myscript'
            }
        stage('Archive') {
            steps {
                archiveArtifacts artifacts: 'output', followSymlinks: false
            }
    }
}

