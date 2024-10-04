pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                C://Users//arnav//miniconda3 conda create -n mlip python pytest numpy pandas scikit-learn -c conda-forge
                C://Users//arnav//miniconda3 conda activate mlip
                '''
            }
        }
        stage('Test') {
            steps {
                sh '''#!/bin/bash
                echo 'Test Step: We run testing tool like pytest here'

                # TODO fill out the path to conda here
                # sudo /PATH/TO/CONDA init

                # TODO Complete the command to run pytest
                # sudo /PATH/TO/CONDA run -n <Envinronment Name> <Command you want to run>
                C://Users//arnav//miniconda3 conda run -n mlip pytest

                echo 'pytest not runned'
                exit 1 #comment this line after implementing Jenkinsfile
                '''

            }
        }
        stage('Deploy') {
            steps {
                echo 'In this step, we deploy our porject'
                echo 'Depending on the context, we may publish the project artifact or upload pickle files'
            }
        }
    }
}
