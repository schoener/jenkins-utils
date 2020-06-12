# jenkins-utils
* to get the crumb for issuing jenkins `curl -s -u username:<API token or password> http://localhost:8081/crumbIssuer/api/json`
* to fire a jenkins job `curl -X POST http://localhost:8081/job/test-multibranch-pipeline/job/master/build -u username:<API token or password> -H 'Jenkins-Crumb: <Generated Jenkins-Crumb from the call above>'`
