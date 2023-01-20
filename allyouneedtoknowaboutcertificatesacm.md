ACM Certificates
OpenShift Certificates
Replacing Custom Certificates
Expired Certificates
Common Questions
CertManager Integration
CertificateController Integration


we plan to exchange the ingress and API certificate (which has been created during the cluster setup and is self-signed) of our ACM hub cluster.
For this we will use a certificate which is signed by our company CA.
We currently have many running managed cluster controlled by our ACM hub prod cluster.


https://access.redhat.com/documentation/en-us/red_hat_advanced_cluster_management_for_kubernetes/2.6/html-single/governance/index#certificates

https://docs.openshift.com/container-platform/4.11/security/certificates/replacing-default-ingress-certificate.html

https://access.redhat.com/documentation/en-us/red_hat_advanced_cluster_management_for_kubernetes/2.6/html-single/install/index#custom-ca-configma

https://access.redhat.com/documentation/en-us/red_hat_advanced_cluster_management_for_kubernetes/2.6/html-single/multicluster_engine/index#troubleshooting-imported-clusters-offline-after-certificate-change-mce

https://access.redhat.com/documentation/en-us/red_hat_advanced_cluster_management_for_kubernetes/2.6/html-single/troubleshooting/index#troubleshooting-imported-clusters-offline-after-certificate-change


The first three are documentation related to the operation, the last two are troubleshooting documentation we have regarding what can happen.


If you have enabled observability you may also want to check https://access.redhat.com/documentation/en-us/red_hat_advanced_cluster_management_for_kubernetes/2.6/html-single/observability/index#customizing-route-cert and take that into consideration, but that probably isn't needed here.



