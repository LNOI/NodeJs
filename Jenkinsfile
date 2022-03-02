pipeline{
    agent any
    stages{
        stage("init"){
            try{
                sh 'node -v'
                sh 'npm -v'
            }
            catch{
                sh  'echo "npm not found!"'
            }
           
        }
    }
}