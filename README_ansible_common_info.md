# About Ansible
Ansible is an open-source software provisioning, configuration management, and application-deployment tool enabling infrastructure as code (IaC). It runs on many Unix-like systems, and can configure both Unix-like systems as well as Microsoft Windows. It includes its own declarative language to describe system configuration. 

<img src="https://user-images.githubusercontent.com/67045661/172068140-32d5679e-a821-4b80-b180-2782ab7fb576.png" width="750" height="400">

### [Ansible is](https://habr.com/ru/company/otus/blog/570926/):
- **Agentless**: The IAC tool may require you to run an agent on each server that you want to configure. If not, then such a tool is called "agentless".
- **Mutable**: Some tools, such as Terraform, are not about modifying an already provisioned infrastructure, but deploying a new server, which means that they follow the immutable infrastructure paradigm. Other tools such as Ansible, Chef, SaltStack, and Puppet can modify existing resources, which means that these tools follow the mutable infrastructure paradigm.
- **Procedural languaged**: Procedural languages, such as Ansible and Chef, allow you to describe step-by-step execution in code, while declarative languages, such as Terraform, SaltStack, and Puppet, allow you to simply specify the desired state. 
- **Masterless**: Languages like Chef require you to run a separate master server to provide additional control and persistent states. Other languages such as Ansible and Terraform do not need a wizard definition. 
- **Configuration**: Ansible, Chef, SaltStack and Puppet are known as configuration management tools, which means that their main purpose is to configure resources. Other tools, such as Terraform and Pulumi, are provisioning tools, meaning that their primary purpose is to provide resources. However, as the tools evolve, their functionality may begin to overlap. 

### Minimal requirements 
#### for Control/Master Server:
- Linux only
- Python2.6+ or Python3.5+
#### for Controlled/Managed Servers:
##### **Linux:**
- Admin username and password or SSH key
- Python2.6+ 
##### Windows:
- Admin username and password
- Powershell 3.0+
- Run the [script]()

### Ansible working through the following protocols/ports:
- Linux: SSH, port 22
- Windows: WinRM, port 5986
