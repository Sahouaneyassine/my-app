node{
    stage('SCM Checkout'){
        git 'https://github.com/Sahouaneyassine/my-app'
    }
    
    stage('Compile package'){
        def mvHome = tool name: 'maven-3' , type: 'maven'
        sh "${mvHome}/bin/mvn package"
    }  

}
