Started by user Juan Pablo Monzon
Obtained Jenkinsfile from git https://github.com/jpmonzon/app-pipeline-prc
[Pipeline] Start of Pipeline
[Pipeline] node
Running on Jenkins in /var/jenkins_home/workspace/app-pipeline-prc
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
Selected Git installation does not exist. Using Default
The recommended git tool is: NONE
using credential aff89bd5-5d40-4f6d-a7c5-e146851730c0
 > git rev-parse --resolve-git-dir /var/jenkins_home/workspace/app-pipeline-prc/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/jpmonzon/app-pipeline-prc # timeout=10
Fetching upstream changes from https://github.com/jpmonzon/app-pipeline-prc
 > git --version # timeout=10
 > git --version # 'git version 2.43.0'
using GIT_ASKPASS to set credentials 
 > git fetch --tags --force --progress -- https://github.com/jpmonzon/app-pipeline-prc +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/main^{commit} # timeout=10
Checking out Revision 314a4b0ed6c7b114f50afdc846cd4b79b49b42c2 (refs/remotes/origin/main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 314a4b0ed6c7b114f50afdc846cd4b79b49b42c2 # timeout=10
Commit message: "add Jenkins file"
 > git rev-list --no-walk 314a4b0ed6c7b114f50afdc846cd4b79b49b42c2 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Checkout)
[Pipeline] git
Selected Git installation does not exist. Using Default
The recommended git tool is: NONE
No credentials specified
 > git rev-parse --resolve-git-dir /var/jenkins_home/workspace/app-pipeline-prc/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/jpmonzon/app-pipeline-prc.git # timeout=10
Fetching upstream changes from https://github.com/jpmonzon/app-pipeline-prc.git
 > git --version # timeout=10
 > git --version # 'git version 2.43.0'
 > git fetch --tags --force --progress -- https://github.com/jpmonzon/app-pipeline-prc.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/main^{commit} # timeout=10
Checking out Revision 314a4b0ed6c7b114f50afdc846cd4b79b49b42c2 (refs/remotes/origin/main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 314a4b0ed6c7b114f50afdc846cd4b79b49b42c2 # timeout=10
 > git branch -a -v --no-abbrev # timeout=10
 > git branch -D main # timeout=10
 > git checkout -b main 314a4b0ed6c7b114f50afdc846cd4b79b49b42c2 # timeout=10
Commit message: "add Jenkins file"
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Install Dependencies)
[Pipeline] sh
+ npm install
/var/jenkins_home/workspace/app-pipeline-prc@tmp/durable-4ffa9e1f/script.sh.copy: line 1: npm: not found
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Build)
Stage "Build" skipped due to earlier failure(s)
[Pipeline] getContext
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Test)
Stage "Test" skipped due to earlier failure(s)
[Pipeline] getContext
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Deploy)
Stage "Deploy" skipped due to earlier failure(s)
[Pipeline] getContext
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Pipeline failed.
[Pipeline] }
[Pipeline] // stage
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // node
[Pipeline] End of Pipeline
ERROR: script returned exit code 127
Finished: FAILURE
