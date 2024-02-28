# Azure Repos - install and configure and configure using Helm

{% hint style="info" %}
**Feature availability**

Snyk Azure Repos are available only for Azure DevOps/TFS 2020 or above.
{% endhint %}

Before installing, review the prerequisites and the general instructions for installation using [Helm](../install-and-configure-broker-using-helm.md).

To use this chart, you must first add the Snyk Broker Helm Chart by adding the repo:

`helm repo add snyk-broker https://snyk.github.io/snyk-broker-helm/`&#x20;

Then run the following commands to customize the environment variables. Refer to [Azure Repos - environment variables for Snyk Broker](azure-repos-environment-variables-for-snyk-broker.md) for definitions of the environment variables.

Note that for the variable `azureReposHost` the value does not include `https://`. If you have more than one Azure organization, you must deploy a Broker for each one. Snyk AppRisk is set by default to **`false`**. Enable it by setting the flag to **`true`**.

```
helm install snyk-broker-chart snyk-broker/snyk-broker \
             --set scmType=azure-repos \
             --set brokerToken=<ENTER_BROKER_TOKEN> \
             --set azureReposToken=<ENTER_REPO_TOKEN> \
             --set azureReposOrg=<ENTER_REPO_ORG> \
             --set azureReposHost=<ENTER_REPO_HOST> \
             --set brokerClientUrl=<ENTER_BROKER_CLIENT_URL>:<ENTER_BROKER_CLIENT_PORT> \
             --set enabledAppRisk=true \
             -n snyk-broker --create-namespace
```