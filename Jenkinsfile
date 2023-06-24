pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs ‘nodejs’ 
    }
    

    stages{
        stage(‘Build’){
            steps{
                echo 'this is the first job - Build’
                sh ‘npm install’
            }
        }
        stage(’Test’){
            steps{
                echo 'this is the second job - Test’
                sh ‘npm test’
            }
        }
        stage(‘Package’){
            steps{
                echo 'this is the third job - Package’
                sh ‘npm run package’
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}