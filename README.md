## Jenkins-Project-Scripts
Jenkins is a popular automation server used by development teams for continuous integration and continuous delivery (CI/CD) purposes. As Jenkins evolves, it is crucial to keep your Jenkins server up-to-date to benefit from the latest features, improvements, and security updates.
### Build Commands 
- Source code validation aka scanning `mvn validate`
- Compile your source code `mvn compile`or `mvn clean install`
- Run project unit testing with `mvn test`
### Create a plugin from the Jenkins Template
- `mvn -U archetype:generate -Dfilter="io.jenkins.archetypes:"`
- Verify your project build `mvn verify` and package the project `mvn package`
- Move `.hpi` file from targets to `Jenkins Plugin Directory` and `Restart the Jenkins Service`
- LogIn Jenkins and follow below steps: `New freestyle job`, Add `"Hello World" build step` and `Run, check console`