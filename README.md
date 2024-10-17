Hi folks, here’s how to get you started on the templates:

    oc new-project myregistry
    oc create secret docker-registry docker \--docker-username \<user\>  \--docker-password \<password\>  \--docker-server docker.io
    oc import-image mysql:5.7 \--confirm \--reference-policy local
    oc new-project \<project\>
    oc apply \-f quotes.yaml
    watch oc get pod

This should work out of the box, please let me know otherwise\!