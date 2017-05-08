node {
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      checkout scm
   }
   stage('Test') {
      // Run the maven build
      sh "molecule test"
   }
   stage('Merge') {
      // Run the maven build
      sh 'git merge develop'
      sh 'git commit -am "Merged develop branch to master'
      sh "git push origin master"
   }
}
