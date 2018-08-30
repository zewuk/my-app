node {
     stage('SCM checkout') {
         git 'https://github.com/zewuk/my-app/'
     }
     stage('Compile-Package){
         sh 'mnv package'
     }
}
