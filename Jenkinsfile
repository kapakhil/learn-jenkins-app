pipeline {
    agent any
    stages {
        stage ('Build') {
            agent {
                docker {
                    image 'node:18-alphine'
                }

                steps {
                    sh ''' 
                        echo "building the project"
                        npm --version
                        node --version
                        npm build
                    '''
                }
            }
        }
    }
}