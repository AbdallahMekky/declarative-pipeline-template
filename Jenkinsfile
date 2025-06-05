pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'chmod a+x run_build_script.sh'
        sh './run_build_script.sh'
      }
    }
    stage('Test') { // Now correctly inside the 'stages' block
      steps {
        echo "Run tests"
      }
    }
  } // Correct closing for 'stages' - now encompassing both 'Build' and 'Test'
} // Correct closing for 'pipeline'
