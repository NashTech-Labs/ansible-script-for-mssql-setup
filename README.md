
# Ansible MSSQL Server Setup

This repository contains Ansible playbooks for setting up and securing a Microsoft SQL Server (MSSQL) database server. The playbooks automate the installation of MSSQL server, configure the database, and apply security measures to ensure a secure setup.

## Prerequisites

Before running the playbooks, ensure the following prerequisites are met:

- Ansible is installed on the control node.
- Access to target MSSQL database server(s) via SSH or WinRM.
- Proper network connectivity between the control node and MSSQL server(s).
- SSH key-based authentication or valid credentials for SSH authentication.

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone <url>
   ```

2. Navigate to the cloned repository directory:

   ```bash
   cd ansible-mssql-setup
   ```

3. Update the `hosts` file to specify the target MSSQL server(s) hostname or IP address.

4. Execute the Ansible playbook:

   ```bash
   ansible_mssql_setup.yml
   ```

5. Follow the prompts and provide necessary inputs when running the playbook.

## Playbook Structure

- The `ansible_mssql_setup.yml` file contains the main Ansible playbook for setting up MSSQL server.
- Tasks are organized into logical sections such as updating packages, configuring firewall, installing MSSQL server, configuring the database, and securing MSSQL server.

## Customization

- Customize the playbook according to your specific requirements, such as MSSQL version, database configurations, and security settings.
- Update the `hosts` file to define the target MSSQL server(s) and their corresponding connection parameters.
