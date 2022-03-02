pipeline{
    agent any
    stages{
        stage("init"){
            steps{
                script{
                    try{
                        sh 'sudo apt-get install nodejs'
                        sh 'node -v'
                    }
                    catch(error){
                        
                        sh  'echo "npm not found!"'
                    }
                }
            }
            
           
        }
    }
}