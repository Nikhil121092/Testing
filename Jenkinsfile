pipeline{
    agent any
    stages{
        stage('Compile'){
            steps{
                echo 'Compiled Successfully';
            }
        }
        stage('Build Compiled Code'){
            steps{
                echo 'Build Successfully';
            }
        }
        stage('Unit Testing'){
            steps{
                echo 'Unit Test Successfully';
            }
        }
        stage('Sonar Check'){
            steps{
                echo 'Sonar Check Successfully';
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployment Successfully';
            }
        }
    }
    post{
        always{
            echo 'This will always run'
        }
        success{
            echo 'This will run only if success'
        }
        failure{
            echo 'This will run only if failed'
        }
        unstable{
            echo 'This will run only if the run was marked as unstable'
        }
        changed{
            echo 'This will run only if the state of pipeline is changed'
        }
    }
}
