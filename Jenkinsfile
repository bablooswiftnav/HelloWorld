pipeline{
    agent any    
    stages{
        stage("Image Building"){
            steps{
                script{
                    echo 'Building Image'
                    sh 'docker build -t babloojangoo/hello0 .'
                }
            }
        }
        stage("Image Running"){
            steps{
                script{
                    echo 'Running Image'
                    sh 'docker run  babloojangoo/hello0'
                }
            }
        }
        stage("Testing"){
            steps{
                echo "first statge"
            }
        }
    }
}
