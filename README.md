# maven-test-app
Maven application to test Ci/CD pipeline

### How to run locally
1. git clone https://github.com/kuttor/maven-test-app
2. cd maven-test-app
3. mvn compile
4. java -cp target/classes com.DimensionData.app.App

### Purpose of repo
This repository is connected with a Jenkins build to demonstrate an automatice code deploy based on a git push

### Pipeline order-of-operations
1. Developer pushes change to Git Repo
2. Git repo sends update to Jenkins
3. Jenkins job starts building the updated code
4. Completed build is deployed to Artifactory
5. Jenkins job alerted of Artifact update and deploy job starts
6. Deploy job sends updated code to the VMs

### Reference
[Maven in 5 Minutes](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html)
[Artifactory User Guide](https://www.jfrog.com/confluence/display/RTF/Welcome+to+Artifactory)

