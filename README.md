# Jenkins Node Labeler

Adds a bunch of labels to macOS nodes in Jenkins.

- macOS version (`sw_vers -productVersion`)
- XCode version and XCode major version (`xcodebuild -version`)
- node name (`hostname`)
- system architecture (`uname -m`)
- additional labels

examples
`'iOS', 'xcode-13.1', 'xcode-13', 'macos-12.1', 'node-ios-build1', 'arch-arm64'`

## Settings
```
JENKINS_USERNAME="some_user"
JENKINS_APIKEY="API_KEY" #See https://www.jenkins.io/blog/2018/07/02/new-api-token-system/
JENKINS_HOST="https://jenkins.example.com"
JENKINS_ADDITIONAL_LABELS="Some-Label Other-label"
```