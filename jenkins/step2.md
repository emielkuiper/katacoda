Create job item, example "CICD Simulation" and select Pipeline. After that just click OK.

In "Advanced Project Options" write the pipeline script like below:
`
pipeline {
    agent none
    stages {
        stage('Version Control') {
            steps {
                echo "Run Step 1"
            }
        }
        stage("Build") {
            steps {
                echo "Run Step 1"
            }
        }
        stage('Unit Test') {
            parallel {
                stage('Functional Testing') {
                    steps {
                        echo "Run Step 1"
                    }
                }
                stage('Security Testing') {
                    steps {
                        echo "Run Step 1"
                    }
                }
            }
        }
        stage("Deploy Staging") {
            steps {
                echo "Run Step 1"
            }
        }
        stage('Auto Test') {
            steps {
                echo "Run Step 1"
            }
        }
        stage("Deploy Production") {
            steps {
                echo "Run Step 1"
            }
        }
        stage('Measure & Validate') {
            steps {
                echo "Run Step 1"
            }
        }
    }
}
`{{copy}}

Have done? let run it with click Build Now.