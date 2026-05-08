# flowset-help

Helm Charts for Flowset

## How to install
### Add the Helm Chart Repository
To add the Helm chart repository for Flowset, run:

```shell
helm repo add flowset https://dlr-terrabyte.github.io/flowset-helm/
```

### Verify the Repository
To confirm that the repository has been added successfully, list all available repositories:

```shell
helm repo list
```

### Update Helm Repositories
Fetch the latest available chart versions by updating your Helm repositories:

```shell
helm repo update
```

### List Available Flowset Versions

To check the available versions of the Flowset chart, use the following command:

```shell
helm search repo flowset --devel
```

The output should be something like:

```
NAME                    CHART VERSION   APP VERSION     DESCRIPTION
flowset/flowset-control 0.1.0           1.16.0          Helm chart for Flowset
```

Note: The `--devel` flag includes development versions in the search results. Without this flag, only stable versions will be listed.

### Install a Specific Version

To install a specific version from the list above, use:

```shell
helm install flowset-control flowset/flowset-control --version 0.1.0
```
