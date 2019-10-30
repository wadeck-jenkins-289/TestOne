echo 'hello from Pipeline'

withCredentials([usernameColonPassword(credentialsId: 'wadeck-pat', variable:'PAT')]){
  echo "${PAT.split('').join(' ')}"
}
