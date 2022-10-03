Java application and Tekton Pipeline integrations
===================

Tools
-------------------
* OCP 4.8.2

How To
--------------------
``` 
oc create -f 01.pvc.yml -n tekton-springboot-pipeline
oc create -f 02.pipeline.yml -n tekton-springboot-pipeline
oc create -f 03.task-git-clone.yml -n tekton-springboot-pipeline
oc create -f 04.task-mvn.yml -n tekton-springboot-pipeline
oc create -f 05.task-deploy-and-clean.yml -n tekton-springboot-pipeline
oc create -f 06.pipeline-run.yml -n tekton-springboot-pipeline
```

Java Code
--------------------
Spring Boot code are taken from below repository
```
https://github.com/edwin/spring-boot-hello-world
```

Blog Post
--------------------
```
https://edwin.baculsoft.com/2021/11/deploy-a-java-application-to-openshift-by-using-tekton-pipeline/
```
