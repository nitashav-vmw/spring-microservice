# spring-microservice

## Need a new namespace in your cluster?
Click [here](https://github.com/cdelashmutt-pivotal/gbs-gitops/new/main?filename=config/nitashav.yaml&message=New%20Developer%20Namespace&value=apiVersion%3A%20v1%0Akind%3A%20Namespace%0Ametadata%3A%0A%20%20labels%3A%0A%20%20%20%20apps.tanzu.vmware.com%2Ftap-ns%3A%20%27%27%0A%20%20name%3A%20nitashav) to add a new namespace for development.

## Getting access to environment
First, make sure you have downloaded the TMC CLI from https://fiservesf.tmc.cloud.vmware.com/automation/cli, and follow the instructions on that page to create an API key for your account, and login to TMC with the TMC CLI.

Next, Click [here](https://fiservesf.tmc.cloud.vmware.com/clusters) to access your clusters in TMC.  Click on the name of your cluster, and select the "Actions" -> "Access this cluster" function to download a kubeconfig file for enabling access to the development environment.  Follow the instructions on the page to move your kubeconfig to `%USERPROFILE%\.kube\config` for Windows, or `~/.kube/config` for WSL and Linux.

## Register your app with the TAP Catalog
Copy the URL to your [catalog/catalog-info.yaml](catalog/catalog-info.yaml), and paste the URL into the page at https://tap-gui.20-75-114-95.nip.io/catalog-import