 pipeline{
    agent any
    // options { skipDefaultCheckout()}
    stages{

        // stage('Checkout'){
        //     steps{
        //         git url: 'https://github.com/ganislp/jenkins-demo-project.git',branch: 'main'
        //         sh "ls -ltr"
        //     }

        // }
        stage('Setup'){
            steps{
                sh "pip install -r requirements.txt"
            }
        }

        stage('Test'){
            steps{
               sh "pytest"
            }
        }

}

}