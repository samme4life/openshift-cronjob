## YAML File to create a CronJob in OpenShift
This codebase contains the YAML file which contains the cronjob information to be imported into OpenShift project

The API Document can be found at "https://app.swaggerhub.com/apis/samme4life/user-rego/0.0.1"

## Reference

* OpenShift Documentation on Jobs & Cron Jobs: "https://docs.openshift.com/container-platform/4.1/nodes/jobs/nodes-nodes-jobs.html"
* StackOverflow Thread I raised: "https://stackoverflow.com/questions/60135077/run-a-kubernetes-cron-job-from-openshift-to-call-a-rest-endpoint-periodically"
* StackOverflow Thread I found the solution: "https://stackoverflow.com/questions/47203080/call-endpoint-from-kubernetes-cron-job"
	
## Important OC commands

* login to a certain OpenShift cluster: oc login --server=<server-url>
	
    Then provide relevant un and pw
* to delete a cron-job: oc delete cronjob/<cron_job_name>
	
