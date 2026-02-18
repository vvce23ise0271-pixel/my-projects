pipeline{
  agent any

  stages{

    stage('Clone'){
      steps{
        git url: 'https://github.com/vvce23ise0271-pixel/my-projects.git',
        branch: 'main'
      }
    }

    stage('Run Script'){
      steps{
        sh 'sed -i -e "s/\r$//" script.sh'
        sh 'chmod +x script.sh'
        sh './script.sh'
      }
    }
  }
}
