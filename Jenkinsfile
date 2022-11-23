pipeline {
  agent any	
  stages {
	  parameters {
  choice choices: ['git', 'tree', 'vim', 'gcc', 'make'], description: 'To install package in Ubuntu Machine', name: 'Select_Package'
}
    stage ('BUILD') {
      steps {
	      echo "To install package ${params.Select_Package}"
        sh '''
	sudo apt install $select_Package
	'''
      }  
    }  
        }
}
