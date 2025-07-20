#  Ansible Zero Bootstrap 🚀

![Admin Terraform Bootstrap EC2 Demo](https://raw.githubusercontent.com/AlexandrNeverov/ansible-zero-node/main/image.png)

## 🚀 Why This Matters

Setting up a secure, automation-ready EC2 instance with Ansible and DevOps tools usually takes multiple steps: SSH key generation, Ansible installation, environment configuration, and CLI tool setup — all done manually.

Ansible Zero Bootstrap automates this entire process in structured scripts:
	•	You get an EC2 instance launched with an IAM Instance Profile (no static credentials)
	•	Ansible is installed from the official PPA and ready to run
	•	All essential CLI tools are preinstalled (Git, jq, AWS CLI, Python, etc.)
	•	SSH key is generated and exported to your local project directory
	•	Vault can optionally be installed and launched as a systemd service

This is ideal for:
	•	🧪 Ansible testing, learning, and quick-start labs
	•	💡 Building reproducible DevOps environments in the cloud
	•	🔁 Fast, zero-touch provisioning of EC2 nodes for automation workflows
	•	🔐 Secure AWS setups with IAM roles (no hardcoded access keys)

---

## ✅ Features

	•	🖥️ EC2 provisioning with admin IAM role and metadata-based auth
	•	🔧 Installation of Ansible via official Ubuntu PPA
	•	🧰 Preinstalled CLI tools:
	•	AWS CLI v2, Git, jq, curl, unzip, htop, tmux, Python3, pip3
	•	⏰ Timezone configuration (America/New_York) via timedatectl
	•	🗂️ Directory setup: ~/projects/ansible, ~/projects/terraform, and IP logging
	•	🔑 SSH key generation and export to ~/projects/ssh.pub
	•	🔐 Optional: Vault installation with systemd service and minimal config
	•	🧱 Modular design: scripts are reusable individually or as a full pipeline

> All operations are performed through CLI and AWS APIs. No manual interaction after launch. Ideal for repeatable cloud automation workflows.
> All actions are performed via CLI using official AWS APIs and require only existing access credentials with IAM privileges.
