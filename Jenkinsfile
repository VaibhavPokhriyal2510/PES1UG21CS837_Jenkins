pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG21CS837_vaibhav.cpp' // changing file name here
                sh 'g++ -o PES1UG21CS837 PES1UG21CS837.cpp'
                echo 'build stage successful'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG21CS837'
                echo 'Test stage executed successfully'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployed Successfully'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
