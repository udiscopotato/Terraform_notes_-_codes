# Some Questions and Answers
Frequently asked in interview and exams.

### 1. What's IaC ?
Infrastructure as Code(IaC) is the practice of provisioning and managing IT infrastructure using code rather then manual aproach.

### 2. What're the benifits of IaC ?
Iac provides many benifits in compare to traditional manual provision
- Automation: IaC automates the process of setting up and managing environments, reducing manual effort and human error.
- Consistency: IaC ensures that your infrastructure is consistent across different environments (development, testing, production).
- Scalability: Easily duplicate environments or scale resources up or down using the same code.
- Version Control: Infrastructure code can be versioned and tracked in source control systems (e.g., Git).

### 3. What's IaC tool, give some examples ?
IaC tools are software solutions that enable the automation of infrastructure provisioning and management. They use code to automate the setup and configuration of IT resources, making it easier to manage large-scale. 
Some Examples are: Terraform(open-source),Ansible(open-source),Puppet(open-source),Chef,AWS Cloud Formation, and manymore.

### 4. Why Terraform ?
Terraform is an Open-source Infrastructure as Code(IaC) tool developed by HashiCorp. It's popular due to it's vast integration and adaption to most of cloud providers.

### 5. In which language Terraform configuration files are written ?
Terraform configuration files are written in the Terraform language, also known as HashiCorp Configuration Language (HCL). It's a Declarative language with ".tf" file extension.

### 6. state some differences between terraform and ansible ?
- Terraform is primarily focused on provisioning and managing infrastructure resources. while Ansible focuses on configuration management, application deployment, and task automation.
- Terraform configuration files are written in HCL while Ansible playbooks are written in YAML.
- Terraform is Agentless while Ansible performs all tasks inside Agents via SSH.
- Terraform maintains a State-file to trach resource changes but Ansible is Stateless it does not maintain states.

### 7. What's is Terraform Resource ?
Terraform resources are components within a Terraform configuration that represent infrastructure objects or services that need to be managed. In sort Resources are all those infrastructure that terraform manage.

### 8. What're the phases in terraform ?
Terraform has 5 main phases: Write, Init, Plan, Apply, and Destroy.

### 9. What do Terraform do in the init stage ?
initializes a working directory and downloads the necessary provider plugins and modules and setting up the backend for storing your infrastructure's state.

### 10. What do Terraform do in the plan stage ?
creates a dry-run, determining what actions are necessary to achieve the desired state defined in the Terraform configuration files.

### 11. What do Terraform do in the apply stage ?
applies the changes required to reach the desired state of the configuration, thereby creating, modifying, or deleting the infrastructure resources as necessary.

### 12. What do Terraform do in the destroy stage ?
