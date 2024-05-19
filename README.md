Started by user Juan Pablo Monzon
Obtained Jenkinsfile from git https://github.com/jpmonzon/app-pipeline-prc
[Pipeline] Start of Pipeline
[Pipeline] node
Running on Jenkins in /var/jenkins_home/workspace/app-pipeline-prc@2
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
Selected Git installation does not exist. Using Default
The recommended git tool is: NONE
using credential aff89bd5-5d40-4f6d-a7c5-e146851730c0
 > git rev-parse --resolve-git-dir /var/jenkins_home/workspace/app-pipeline-prc@2/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/jpmonzon/app-pipeline-prc # timeout=10
Fetching upstream changes from https://github.com/jpmonzon/app-pipeline-prc
 > git --version # timeout=10
 > git --version # 'git version 2.43.0'
using GIT_ASKPASS to set credentials 
 > git fetch --tags --force --progress -- https://github.com/jpmonzon/app-pipeline-prc +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/main^{commit} # timeout=10
Checking out Revision eed4530a74d980563de7f12c2ef4f22409d8d7f0 (refs/remotes/origin/main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f eed4530a74d980563de7f12c2ef4f22409d8d7f0 # timeout=10
Commit message: "Update Jenkinsfile"
 > git rev-list --no-walk eed4530a74d980563de7f12c2ef4f22409d8d7f0 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Tool Install)
[Pipeline] tool
[Pipeline] envVarsForTool
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Preparation)
[Pipeline] tool
[Pipeline] envVarsForTool
[Pipeline] withEnv
[Pipeline] {
[Pipeline] sh
Warning: JENKINS-41339 probably bogus PATH=/var/jenkins_home/tools/jenkins.plugins.nodejs.tools.NodeJSInstallation/my-node/bin:/var/jenkins_home/tools/jenkins.plugins.nodejs.tools.NodeJSInstallation/my-node/bin:PATH = "/usr/bin:PATH = "/usr/bin:$PATH""; perhaps you meant to use ‘PATH+EXTRA=/something/bin’?
process apparently never started in /var/jenkins_home/workspace/app-pipeline-prc@2@tmp/durable-67d781c6
(running Jenkins temporarily with -Dorg.jenkinsci.plugins.durabletask.BourneShellScript.LAUNCH_DIAGNOSTICS=true might make the problem clearer)
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Install Dependencies)
Stage "Install Dependencies" skipped due to earlier failure(s)
[Pipeline] getContext
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Pipeline finished.
[Pipeline] echo
Pipeline failed.
[Pipeline] }
[Pipeline] // stage
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // node
[Pipeline] End of Pipeline
ERROR: script returned exit code -2
Finished: FAILURE
