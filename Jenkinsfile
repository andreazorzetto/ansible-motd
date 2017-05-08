node {
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/andreazorzetto/ansible-motd.git'
   }
   stage('Build') {
      // Run the maven build
      sh "molecule test"
   }
}
