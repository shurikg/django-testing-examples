pipeline {
    agent {
        docker {
            image 'python:3.9' // Docker image to use
        }
    }

    stages {

        stage('Requirements') {
            steps {
                sh 'pip install -r testing-requirements.txt' // Install dependencies from requirements.txt
            }
        }

//         stage('Test') {
//             steps {
//                 dir('rewear//Rewear//rewear_project//main'){
//                  // Change to the rewear_project directory
// //                     sh 'pipenv run python manage.py test' // Specify the path to manage.py
//                     sh 'python tests.py'
//                 }
//             }
//         }



//         stage('Deploy') {
//             steps {
//                 sh 'pipenv run python manage.py migrate'
//                 sh 'nohup pipenv run python manage.py runserver & sleep 5'
//                 sh 'pipenv run python manage.py test'
//                 script {
//                     def processIds = sh(script: "ps aux | grep 'python manage.py runserver' | grep -v grep | awk '{print \$2}'", returnStdout: true).trim()
//                     if (processIds) {
//                         sh "echo '${processIds}' | xargs -r kill -9"
//                     }
//                 }
//             }
//         }
    }
}