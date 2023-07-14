# About

This repositoriy provides the base manifests to deploy Red Hat Build of Apicurio Registry, together with a Red Hat Single Sign-On instance to provide OAuth authentication and authorization for it and a Kafka Cluster based on AMQ Streams used to store its data. This deployment meant for quickly testing the Apicurio Registry and **it's NOT intended for production environments**. 

# Requirements

You'll require an OpenShift cluster with the following OLM operators installed:
* Red Hat Service Registry
* Red Hat AMQ Streams
* Red Hat Single Sign-On

# How

Update the route of Keycloak in `manifests/apicurio.yaml` with your specific Keycloak route and then just apply the manifests.

```
oc apply -f manifests/
```
