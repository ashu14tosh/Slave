pipeline {
  agent {
    label {
      label'built-in'
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
            sh "cp -r /mnt/newslave/index.html /var/www/html"
                
      }
    }
    
  }
}
