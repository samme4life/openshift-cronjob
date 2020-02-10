## YAML File to create a CronJob in OpenShift
This is a result of a research done on "How to Deploy a Srping Batch Operation on OpenShift and Execute it periodically using a CronJob".

The other related codebase resides at "https://github.com/samme4life/spring-batch-example"

This codebase contains the YAML file which contains the cronjob information to be imported into OpenShift project

## Reference

* OpenShift Documentation on Jobs & Cron Jobs: "https://docs.openshift.com/container-platform/4.1/nodes/jobs/nodes-nodes-jobs.html"
* StackOverflow Thread I raised: "https://stackoverflow.com/questions/60135077/run-a-kubernetes-cron-job-from-openshift-to-call-a-rest-endpoint-periodically"
* StackOverflow Thread where I found the solution: "https://stackoverflow.com/questions/47203080/call-endpoint-from-kubernetes-cron-job"
	
## Important OC commands

* login to a certain OpenShift cluster: oc login --server=<server_url>
* to delete a cron-job: oc delete cronjob/<cron_job_name>
	
