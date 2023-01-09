pipeline{
    agent any

    stages{

        stage('git checkout'){

            steps{
                git 'https://github.com/satish855/demo-app.git'
            }
        }
        stage('unit testing'){

            steps{
                sh 'mvn test'
            }
        }
        stage('integration testing){

            steps{
                sh 'mvn verifiy -DskipUnitTests'
            }
        }

    }
}
