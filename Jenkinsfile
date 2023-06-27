pipeline{
    agent any
    stages{
        stage('1-test-git'){
            steps{
                echo "unit testing"
            }
        }
        stage('2-build'){
            steps{
                echo "building...."
            }
        }
        stage('3-pr-test'){
            steps{
                echo "mvn"
            }
        }
    }
}