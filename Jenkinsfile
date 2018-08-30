node {
     stage('SCM checkout') {
         git 'https://github.com/zewuk/my-app/'
     }
     stage('Compile-Package'){
         def mvnHome = tool name: 'maven-3', type: 'maven'
          sh " ${mvnHome}/bin/mvn package"
     }
}
