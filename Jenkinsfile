pipeline{
    agent any    
    stages{
        stage("git checkout"){
            steps{
                echo "first statge"
            }
        }
        stage("Run docker image"){
            steps{
                script{
                    echo 'Building Image'
                    sh 'docker build -t babloojangoo/hello0 .'
                    }
                }
            steps{
                script{
                    echo 'Running Image'
                    //  sh 'mount --bind /media/daten/home/hellouniverse /home/hellouniverse'
                    sh 'docker run  babloojangoo/hello0'
                    // sh 'docker run -it --home=/ babloojangoo/hellouniverse'
                    // sh 'docker run --mount type=bind,source=/home/hellouniverse,target=/data hellouniverse-image'
                }
            }
        }
    }
}
