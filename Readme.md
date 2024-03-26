## Jenkins Job Configuration for Ansible Playbook Execution

This Jenkins job is designed to execute an Ansible playbook named `foobar.yaml` using the provided inventory file. Before running the job, ensure you have the necessary prerequisites installed on your Jenkins environment, including Ansible and any required plugins.

## String Parameters

When configuring the Jenkins job, the following string parameters should be provided:

### VERSION OF  KUBERNETES 

Specify the version of the playbook or application that you intend to deploy. This parameter allows for version-specific deployments.

### MASTER IP

Provide the IP address of the master node in your target environment. This IP address will be used by Ansible to connect to the master node and execute tasks defined in the playbook.

### WORKER 1 IP

Specify the IP address of the first worker node in your target environment. If your playbook requires interaction with multiple nodes, this parameter allows you to specify the IP address of the first worker node.

### WORKER 2 IP (Optional)

If applicable, provide the IP address of the second worker node in your target environment. This parameter is optional and should only be provided if your playbook requires interaction with a second worker node.

## Example Usage

To execute the Jenkins job, follow these steps:

1. Navigate to the Jenkins web interface and locate the job named Cluster creation using ansible.
2. Click on the job to open its configuration page.
3. Fill in the required string parameters:
   - **VERSION**: Specify the version of the application or playbook.
   - **MASTER IP**: Provide the IP address of the master node.
   - **WORKER 1 IP**: Provide the IP address of the first worker node.
   - (Optional) **WORKER 2 IP**: If required, provide the IP address of the second worker node.
4. Click on the "Build Now" button to trigger the job execution.

Upon successful execution, the Ansible playbook will be executed with the provided inventory file, deploying or configuring the application on the specified nodes in your environment.

