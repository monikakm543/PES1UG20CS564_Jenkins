pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS564.cpp'
                sh 'g++ -o PES1UG20CS564 PES1UG20CS564.cpp'
                echo 'build stage successfull'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS564'
                echo 'Test stage executed successfulllllly'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployed Successfulllllly'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
