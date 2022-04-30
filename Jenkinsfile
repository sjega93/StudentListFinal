pipeline{
        agent any
                tools { 
                maven 'default' 
                jdk 'jdk9' 
                }
        stages {
                stage('Checkout'){
                        steps{
                        git branch: 'master',
                        url: 'https://github.com/sjega93/StudentListFinal.git'
                        }
                        }
                stage('Build'){
                        steps{
                                sh 'mvn clean install'
                        }
                }
        }
}
