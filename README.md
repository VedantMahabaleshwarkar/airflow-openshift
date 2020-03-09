# airflow-openshift  

Deploys the following components to get Apache Airflow running as an application on a Openshift Cluster.  
1) Airflow Webserver  
2) Airflow Worker  
3) Redis  
4) Postgresql  
5) Celery Flower  

## Command to deploy the file  

`oc process -f airflow.template.yml  | oc create -f -`  

### Note:  
You will need to rsh into the Webserver and Worker Pods and execute `airflow initdb` once the application is deployed.   


### Credentials for the Flower UI:  
flower:flower  

