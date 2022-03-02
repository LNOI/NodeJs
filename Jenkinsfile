pipeline{
    agent any
    stages{
        stage("init"){
            steps{
                script{
                    try{
                        sh 'node -v'
                        sh 'npm -v'
                        sh "ls -la"
                    }
                    catch(error){
                        
                        sh  'echo "npm and nodejs not found!"'
                    }
                }
            }
            
           
        }
    }
}