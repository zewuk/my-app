node {
     stage('SCM checkout') {
         git 'https://github.com/zewuk/my-app/'
     }
     stage('Compile-Package'){
         def mvnHome = tool name: 'maven-3', type: 'maven'
          sh " ${mvnHome}/bin/mvn package"
     }
     stage('Email Notification'){
          mail bcc: '', body: 'This is for Kouami', cc: 'komlan_zewu@hotmail.com', from: '', replyTo: '', subject: 'Jenkins testing KZ', to: 'komlan.zewu@hotmail.com'
     }
}
