pipeline{
    agent any
    stages{
        stage("init"){
            steps{
                script{
                    try{
                    sh 'node -v'
                    sh 'npm -v'
                    }
                    catch(error){
                        sh  'echo "npm not found!"'
                    }
                }
            }
            
           
        }
    }
}