pipeline{
    agent any
    stages{
        stage("init"){
            steps{
                script{
                    try{
                        sh 'node -v'
                        sh 'npm -v'
                        sh "npm install"
                        // sh "echo 'WebHook for project'"
                        sh "echo 'WebHook for project'"
                    }
                    catch(error){
                        
                        sh  'echo "npm and nodejs not found!"'
                    }
                }
            }
        }
        stage("deploy nodejs"){
            steps{
                script{
                    sh 'node index.js'
                    sh 'echo "Deploy success"'
                }
            }
        }
    }
}