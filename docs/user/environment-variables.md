# Environment Variables

The installer accepts a number of environment variable that allow the interactive prompts to be bypassed. Setting any of the following environment variables to their corresponding value, will cause the installer to use that value instead of prompting.

## General

| Environment Variable              | Description                                                                                 |
|:----------------------------------|:--------------------------------------------------------------------------------------------|
| `OPENSHIFT_INSTALL_BASE_DOMAIN`   | The base domain of the cluster. All DNS records will be sub-domains of this base.           |
| `OPENSHIFT_INSTALL_CLUSTER_NAME`  | The name of the cluster. This will be used when generating sub-domains.                     |
| `OPENSHIFT_INSTALL_EMAIL_ADDRESS` | The email address of the cluster administrator. This will be used to log in to the console. |
| `OPENSHIFT_INSTALL_PASSWORD`      | The password of the cluster administrator. This will be used to log in to the console.      |
| `OPENSHIFT_INSTALL_PLATFORM`      | The platform onto which the cluster will be installed.                                      |
| `OPENSHIFT_INSTALL_PULL_SECRET`   | The container registry pull secret for this cluster.                                        |
| `OPENSHIFT_INSTALL_SSH_PUB_KEY`   | The SSH key used to access all nodes within the cluster. This is optional.                  |

## Platform-Specific

| Environment Variable              | Description                                                                              |
|:----------------------------------|:-----------------------------------------------------------------------------------------|
| `OPENSHIFT_INSTALL_AWS_REGION`    | The AWS region to be used for installation.                                              |
| `OPENSHIFT_INSTALL_LIBVIRT_URI`   | The libvirt connection URI to be used. This must be accessible from the running cluster. |