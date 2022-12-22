pipeline {
  agent {
    label {
      label'QA'
      customWorkspace '/mnt/newslave'
          }
  }
  stages {
    stage ('installation'){
      steps {
            sh "sudo yum install httpd -y"
            sh "service httpd start"
      }
    }  
    stage ('deployment'){
      steps {
            sh "cp -r /mnt/assign1/index.html /var/www/html"
                
      }
    }
    
  }
}
